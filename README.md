# Dynamo_Revit
<B>Dynamo Scripts for Revit</B><BR/><BR/>
Questa cartella contiene una libreria di script Dynamo per Revit a disposizione di tutti gli OpenBuilders e si arricchirà ogni qualvolta emergeranno nuove necessità di automazione dei processi progettuali. Potrete scaricare da qui lo script che vi serve e caricarlo in locale per utilizzarlo, segue una breve descizione di ciascuno script corredata dai parametri editabili nel player, la versione Revit e Dynamo e i packages necessari per un corretto funzionamento.

<H2>Family_Data_Cleaner</H2>
<B>Versione Revit:</B> 2022<BR/>
<B>Versione Dynamo:</B> 2.12<BR/>
<B>Packages:</B> Orchid, Clockwork<BR/>
<B>Parametri:</B> Seleziona Tipo Famiglia, Cosa Vuoi Rimuovere?<BR/><BR/>
Lo script consente di eliminare nelle famiglie Revit qualunque riferimento nominale a produttori specifici così da rendere il modello spendibile in Appalto Pubblico. L'automazione rimuove sia i normali parametri di testo che l'eventuale presenza di formule bloccate dal produttore.<BR/><BR/>
<B>Known Issues:</B> Talvolta può essere necessario rilanciare lo script più volte sulla stessa famiglia per rimuovere completamente i parametri.<BR/>

<H2>GuardRail_Profiler</H2>
<B>Versione Revit:</B> 2022<BR/>
<B>Versione Dynamo:</B> 2.12<BR/>
<B>Packages:</B> BimorphNodes, Synthesize Toolkit<BR/>
<B>Parametri(1):</B> Select DWG, Define Layer, Define Picket Family, Set Distance, X/Y/Z Offset<BR/>
<B>Parametri(2):</B> Define Profile Family, Define Profile Name, Define Profile Category<BR/><BR/>
Lo script consente di automatizzare la modellazione di un GuardRail completo su polilinee spaziali. E' disponbile in due versione parziali (solo paletti o solo profilo) e nella forma completa. La polilinea 3D di partenza dovrà essere un file DWG Civil3D hostato in ambiente Revit, per l'inserimento dei paletti basterà selezionare la famiglia da distribuire, il passo tra istanze e l'eventuale offset posizionale nelle 3 dimensioni. Per l'estrusione del GuardRail andrà selezionata una Profile Family specificando la denominazione e la categoria Revit del nuovo oggetto.<BR/><BR/>
<B>Known Issues:</B> Si precisa che all'interno della Profile Family si dovrà eventualmente ruotare e specchiare la sezione sino alla posizione desiderata.<BR/>

<H2>Rooms_to_LineGroups</H2>
<B>Versione Revit:</B> 2022<BR/>
<B>Versione Dynamo:</B> 2.12<BR/>
<B>Packages:</B> Archi-Lab, Clockwork<BR/>
<B>Parametri:</B> -<BR/><BR/>
Lo script automatizza nel file Revit il ricalco dei locali hostati da modelli esterni restituendone i perimetro come gruppi di linee, così da consentire la stampa di una bordatura colorata in base a convenzioni grafiche sulle relative finiture.<BR/><BR/>
<B>Known Issues:</B> Talvolta i gruppi di linee non si autoposizionano, in tal caso andranno inseriti manualmente sui locali dai Gruppi presenti nel Browser.<BR/>

<H2>Set_External_Property</H2>
<B>Versione Revit:</B> 2022<BR/>
<B>Versione Dynamo:</B> 2.12<BR/>
<B>Packages:</B> -<BR/>
<B>Parametri:</B> Categoria Revit, Seleziona File CSV, Parametro Revit di Riferimento e di Destinazione, N. Cella di Riscontro e di Destinazione, Definisci e Sostituisci valori Nulli<BR/><BR/>
Lo script agisce similmente a XLS_Parameter_Compiler ma prelevando i dati da sorgente CSV. Essendo stato sviluppato per una necessità specifica potrebbe richiedere una generalizzazione per altre applicazioni. Il parametro Revit di riferimento verrà ricercato nelle celle di riscontro del file e Dynamo valorizzerà quindi il parametro Revit di destinazione con la relativa cella CSV. Lo script offre inoltre la possibilità di sostituire eventuali valori nulli o indefiniti con una stringa specifica.<BR/>

<H2>Transfer_ViewFilters</H2>
<B>Versione Revit:</B> 2022<BR/>
<B>Versione Dynamo:</B> 2.12<BR/>
<B>Packages:</B> -<BR/>
<B>Parametri:</B> Vista Sorgente, Vista Destinazione, Nome Filtro<BR/><BR/>
Lo script consente di trasferire un determinato Filtro e le sue impostazioni grafiche tra diversi Template Vista, evitando la necessità di una configurazione manuale.<BR/>

<H2>XLS_Parameter_Compiler</H2>
<B>Versione Revit:</B> 2019<BR/>
<B>Versione Dynamo:</B> 2.12<BR/>
<B>Packages:</B> -<BR/>
<B>Parametri:</B> Seleziona File XLS, Nome Foglio, N. Celle Intestazione, N. Cella di Riscontro e da Prelavare, Categoria Revit, Parametro Revit di Riferimento e di Destinazione<BR/><BR/>
Lo script consente di automatizzare la compilazione di un qualsiasi Parametro su una certa categoria Revit a partire da un foglio Excel sorgente. Verranno quindi richiesti il file, il nome del foglio ed il numero di celle intestazione che Dynamo trascurerà. Il numero della cella di riscontro consentirà allo script di creare l'associazione tra il file Excel ed il parametro Revit di riferimento, il numerdo della cella da prelevare andrà quindi a valorizzare il corrispettivo parametro Revit di Destinazione.<BR/>
