# Dynamo_Revit
<B>Dynamo Scripts for Revit</B><BR/><BR/>
Questa cartella contiene una libreria di script Dynamo per Revit a disposizione di tutti gli OpenBuilders e si arricchirà ogni qualvolta emergeranno nuove necessità di automazione dei processi progettuali. Potrete scaricare da qui lo script che vi serve e caricarlo in locale per utilizzarlo, segue una breve descizione di ciascuno script corredata dai parametri editabili nel player, la versione Revit e Dynamo e i packages necessari per un corretto funzionamento.

<H2>Family_Data_Cleaner</H2>
<B>Versione Revit:</B> 2022<BR/>
<B>Versione Dynamo:</B> 2.12<BR/>
<B>Packages:</B> Orchid, Clockwork<BR/>
<B>Parametri:</B> Seleziona Tipo Famiglia, Cosa Vuoi Rimuovere?<BR/><BR/>
Lo script consente di eliminare nelle famiglie Revit qualunque riferimento nominale a produttori specifici così da rendere il modello spendibile in Appalto Pubblico. L'automazione rimuove sia i normali parametri di testo che l'eventuale presenza di formule bloccate dal produttore.<BR/>
<B>Known Issues:</B> Talvolta può essere necessario rilanciare lo script più volte sulla stessa famiglia per rimuovere completamente i parametri.<BR/>

<H2>GuardRail_Profiler</H2>
<B>Versione Revit: 2022</B><BR/>
<B>Versione Dynamo: 2.12</B><BR/>
<B>Packages: BimorphNodes, Synthesize Toolkit</B><BR/>
<B>Parametri (1): Select DWG, Define Layer, Define Picket Family, Set Distance, X/Y/Z Offset</B><BR/><BR/>
<B>Parametri (2): Define Profile Family, Define Profile Name, Define Profile Category</B><BR/><BR/>
Lo script consente di automatizzare la modellazione di un GuardRail completo su polilinee spaziali. E' disponbile in due versione parziali (solo paletti o solo profilo) e nella forma completa. La polilinea 3D di partenza dovrà essere un file DWG Civil3D hostato in ambiente Revit, per l'inserimento dei paletti basterà selezionare la famiglia da distribuire, la relativa distanza ideale e l'eventuale offset posizionale nelle 3 dimensioni. Per l'estrusione del GuardRail andrà selezionata una Profile Family specificando il nome e la categoria Revit del nuovo oggetto.

<H2>Rooms_to_LineGroups</H2>
<B>Versione Revit: 2022</B><BR/>
<B>Versione Dynamo: 2.1</B><BR/>
<B>Packages: Camber</B><BR/>
<B>Parametri: Foglio, ecc ecc</B><BR/><BR/>
Lo script fa questo e questo

<H2>Set_External_Property</H2>
<B>Versione Revit: 2022</B><BR/>
<B>Versione Dynamo: 2.1</B><BR/>
<B>Packages: Camber</B><BR/>
<B>Parametri: Foglio, ecc ecc</B><BR/><BR/>
Lo script fa questo e questo

<H2>Transfer_ViewFilters</H2>
<B>Versione Revit: 2022</B><BR/>
<B>Versione Dynamo: 2.1</B><BR/>
<B>Packages: Camber</B><BR/>
<B>Parametri: Foglio, ecc ecc</B><BR/><BR/>
Lo script fa questo e questo

<H2>XLS_Parameter_Compiler</H2>
<B>Versione Revit: 2022</B><BR/>
<B>Versione Dynamo: 2.1</B><BR/>
<B>Packages: Camber</B><BR/>
<B>Parametri: Foglio, ecc ecc</B><BR/><BR/>
Lo script fa questo e questo
