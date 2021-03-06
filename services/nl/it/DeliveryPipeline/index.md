{:screen: .screen}
{:new_window: target="_blank"}
{:codeblock: .codeblock}
{:shortdesc: .shortdesc}

#Introduzione a {{site.data.keyword.deliverypipeline}} {: #delivery-pipeline}  

*Ultimo aggiornamento: 21 gennaio 2016*

Per automatizzare le tue build e le tue distribuzioni a {{site.data.keyword.Bluemix}}, utilizza IBM Continuous {{site.data.keyword.deliverypipeline}} for {{site.data.keyword.Bluemix_notm}} (il servizio {{site.data.keyword.deliverypipeline}}).
{: shortdesc} 

Quando si sviluppa un'applicazione nel cloud, è possibile scegliere da diversi tipi di build. Fornisci lo script
    di build e {{site.data.keyword.Bluemix_notm}} {{site.data.keyword.jazzhub_short}} lo esegue; non ha bisogno di impostare dei
    sistemi di build. Quindi, con un singolo clic, puoi distribuire automaticamente la tua applicazione a uno o più spazi {{site.data.keyword.Bluemix_notm}}, server Cloud Foundry pubblici o contenitori Docker su IBM Containers for {{site.data.keyword.Bluemix_notm}}.  

I lavori di build compilano e impacchettano il codice sorgente della tua applicazione da repository Git o Jazz SCM (source control management). I lavori di build producono delle risorse utente distribuibili, quali file WAR o contenitori Docker per IBM Containers. Puoi
    inoltre eseguire degli unit test nella tua build automaticamente. Ogni volta che il codice sorgente subisce modifiche,
    viene attivata una build.  

Un lavoro di distribuzione prende l'output da un lavoro di build e lo distribuisce a server IBM Containers o Cloud Foundry come {{site.data.keyword.Bluemix_notm}}.  

Puoi eseguire la distribuzione a uno o più regioni e servizi. Ad esempio, puoi configurare il tuo servizio {{site.data.keyword.deliverypipeline}} in modo che le risorse utente di sviluppo utilizzino IBM Containers, siano testate in un'unica regione e siano distribuite alla produzione in più regioni. Per ulteriori informazioni, consulta [Regioni](../../overview/index.html#ov_intro__reg).

1. Accedi a {{site.data.keyword.Bluemix_notm}}
					e seleziona un'organizzazione e uno spazio per la tua applicazione.
1. Nel Dashboard {{site.data.keyword.Bluemix_notm}}, fai clic su **CREA UN'APPLICAZIONE**.
1. Seleziona un template di applicazione mobile o web, seleziona uno starter e fai clic su
						**CONTINUA**. Fornisci un nome per la tua applicazione e fai clic su
						**FINE**.  
1. Nella pagina Inizia a scrivere codice, scorri la pagina verso il basso e fai clic su **VISUALIZZA PANORAMICA DELL'APPLICAZIONE**.  
1. Nel Dashboard dell'applicazione {{site.data.keyword.Bluemix_notm}}, crea un progetto ospitato da Git per l'applicazione facendo clic su **AGGIUNGI GIT**. Assicurati che la casella di spunta **Popola il repository con il package applicazione starter e abilita {{site.data.keyword.deliverypipeline}} (crea e distribuisci)** sia selezionata e fai clic su **CONTINUA**.   
1. Dopo che il tuo repository Git
					è stato creato, fai clic su **CHIUDI**. Il link AGGIUNGI GIT viene sostituito da un link MODIFICA CODICE e dall'URL del tuo Git.  
1. Aggiungi il servizio {{site.data.keyword.deliverypipeline}}
					allo spazio o agli spazi associati. Dopo che hai aggiunto questo servizio, puoi creare un
     pipeline di distribuzione in più fasi nei tuoi spazi {{site.data.keyword.Bluemix_notm}} configurando
					ed eseguendo le fasi che contengono lavori di build, test e distribuzione.
    1. Nel Dashboard dell'applicazione {{site.data.keyword.Bluemix_notm}}, fai clic su **AGGIUNGI UN SERVIZIO O UNA API**. Per la categoria, seleziona la casella di spunta **DevOps** e, dal catalogo, fai clic su **Delivery Pipeline**.
    2. Seleziona un piano e fai clic su **CREA**. Viene aperto il Dashboard {{site.data.keyword.deliverypipeline}} che mostra l'applicazione da te creata in precedenza.     
  
Nel Dashboard {{site.data.keyword.deliverypipeline}}, puoi visualizzare i tuoi
progetti {{site.data.keyword.jazzhub_short}} e gli stati in cui si trovano. Puoi controllare lo stato delle build, l'applicazione distribuita e le distribuzioni recenti oppure visualizzare i log e i dettagli di
distribuzione più recenti.  

<article class="topic reference nested1" aria-labelledby="d68e338" lang="en-us" id="rellinks">
<h2 class="topictitle2" id="d68e338">Link correlati</h2>
<aside>
<div class="linklist" id="general"><h3 class="linklistlabel">Link correlati</h3>
<ul>
<li><img src="./sout.gif" alt=""><a href="https://developer.ibm.com/bluemix/support/#prereqs" rel="external" title="(Si apre in una nuova scheda o finestra)">Prerequisiti di {{site.data.keyword.Bluemix_notm}}</a></li>
</ul>
</div>

<div class="linklist" id="samples">
<h3 class="linklistlabel">Esercitazioni ed esempi</h3>
<ul>
<li><img src="./sout.gif" alt=""><a href="https://hub.jazz.net/tutorials/devopsweb/" rel="external" title="(Si apre in una nuova scheda o finestra)">Clonare, modificare e distribuire un'applicazione</a></li>
<li><img src="./sout.gif" alt=""><a href="https://hub.jazz.net/tutorials/jazzeditor" rel="external" title="(Si apre in una nuova scheda o finestra)">Sviluppare e distribuire un'applicazione Node.js</a></li>
<li><img src="./sout.gif" alt=""><a href="https://hub.jazz.net/tutorials/jazzeditorjava" rel="external" title="(Si apre in una nuova scheda o finestra)">Sviluppare e distribuire un'applicazione Java</a></li>
<li><img src="./sout.gif" alt=""><a href="http://www.ibm.com/developerworks/topics/delivery%20pipeline%20service" rel="external" title="(Si apre in una nuova scheda o finestra)">developerWorks: servizio {{site.data.keyword.Bluemix_notm}} {{site.data.keyword.deliverypipeline}}</a></li>
</ul>
</div>
</aside>
</article>
