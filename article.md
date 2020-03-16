title: "Mapa i grafy. Podívejte se, jak koronavirus dobyl svět"
perex: "Statisíce nakažených, tisíce mrtvých, ale i více než desítky tisíc zotavených. Koronavirus se už objevil ve více než polovině zemí světa. Prohlédněte si pravidelně aktualizované statistiky epidemie."
coverimg: https://www.irozhlas.cz/sites/default/files/styles/zpravy_snowfall/public/uploader/2020-03-14t161858z_1_200314-185046_mim.JPG?itok=ORA6brdo
coverimg_note: "Foto: Reuters"
styles: ['https://unpkg.com/leaflet@1.6.0/dist/leaflet.css', 'https://data.irozhlas.cz/corona-map/style.css']
libraries: [highcharts, 'https://unpkg.com/leaflet@1.6.0/dist/leaflet.js', 'https://cdnjs.cloudflare.com/ajax/libs/d3/5.15.0/d3.min.js', 'https://data.irozhlas.cz/corona-map/dashboard.js', 'https://data.irozhlas.cz/corona-map/pocitadlo-eu.js', 'https://data.irozhlas.cz/corona-map/pocitadlo-log.js'] #jquery, d3, highcharts, datatables
options: [] #wide, noheader (, nopic)
---
Více než polovina světových zemí ohlásila své nakažené. Onemocnění má původ v Číně, podle Světové zdravotnické organizace se ale nyní ohnisko přesunulo do Evropy. Nejhůře jsou postižené Itálie a Španělsko.

_Počty nakažených ukazuje následující mapa (čísla mají zpoždění přibližně 1 den):_

<wide>
<div id="corona_map"></div>
<script src="https://data.irozhlas.cz/corona-map/script.js"></script>
</wide>

Nejvíce nakažených na kontinentu hlásí Itálie, o řád menší počty pak evidují Španělsko, Francie a Německo.

<wide>
<div id="corona_dboard">
    <div id="corona_dboard_overview">
        <h3>Celková čísla</h3>
        <p>Celkem nakažených: <span id="corona_sum_conf"></span></p>
        <p>Celkem mrtvých: <span id="corona_sum_deaths"></span></p>
        <p>Celkem zotavených: <span id="corona_sum_recov"></span></p>
        <p><span id="corona_stats_updated"></span></p>
    </div>
    <div id="corona_dboard_eu"></div>
    <div id="corona_dboard_world"></div>
</div>
</wide>

Nárůst nakažených ve vybraných evropských státech ilustruje i následující graf nemocných a zemřelých.

<wide>

<div id="corona_eu"></div>
</wide>

Pokud ale chceme vědět, jakou dynamiku epidemie má, absolutní čísla v různě velkých státech nám příliš nepomohou. Pokud například srovnáme Francii s Itálií, můžeme dojít k závěru, že v první jmenované zemi se nic tak zásadního neděje.
Jak ale [vysvětluje John Burn-Murdoch z Financial Times]( https://twitter.com/jburnmurdoch/status/1237748598051409921) , nástup epidemie není lineární, ale spíše logaritmický. Jednoduše řečeno, zpočátku nakažení postupně přibývají, jejich počty ale po čase prudce vystřelí.

Proto je lepší srovnávat státy právě prostřednictvím logaritmické stupnice, a navíc až od 100. nakaženého. Že se pak vývoj epidemie ve většině států vyvíjí podobně, naznačuje následující graf.

<wide>
<div id="corona_log"></div>
</wide>

Všechny podobné grafy a projekce vývoje ale mají jednu zásadní vadu: spoléhají na čísla o počtech nakažených. Jenže ta mohou pokulhávat za realitou, okolo 80 % nakažených má jen lehké příznaky a řada z nich se vůbec nenechá testovat. A to pak může zamávat s každou statistikou, což vysvětluje vědecký novinář Petr Koubský v podcastu Vinohradská 12.

<div class="b-podcast__player">			
      <div class="b-audio-player b-audio-player--podcast js-audio" data-audio-name="irozhlas | iROZHLAS podcast | Zprávy z domova | Petr Koubský: Problém je hlavně v testování. Co nám napovídají dostupná data o koronaviru? || 2020-03-13 | iROZHLAS | 9224909">				
        <div class="js-out">					
          <audio controls="">						
            <source src="https://www.irozhlas.cz/sites/default/files/audios/ffb9f69cd3f29653f3ea621eb36e046d.mp3" type="audio/mpeg">Váš prohlížeč nepodporuje přehrávání audia. 					
          </audio>				
        </div>				
        <div class="b-audio-player__controls">					
          <a href="#" class="b-audio-player__play play-btn">Přehrát 						
            <span class="icon-svg icon-svg--play ">	
              <svg class="icon-svg__svg" xmlns:xlink="http://www.w3.org/1999/xlink">		
                <use xlink:href="https://www.irozhlas.cz/sites/all/themes/custom/irozhlas/img/bg/icons-svg.svg#icon-play" x="0" y="0" width="100%" height="100%">
                </use>	
              </svg>
            </span>						
            <span class="icon-svg icon-svg--pause ">	
              <svg class="icon-svg__svg" xmlns:xlink="http://www.w3.org/1999/xlink">		
                <use xlink:href="https://www.irozhlas.cz/sites/all/themes/custom/irozhlas/img/bg/icons-svg.svg#icon-pause" x="0" y="0" width="100%" height="100%">
                </use>	
              </svg>
            </span>
          </a>					
          <p class="b-audio-player__time">00:00 / 21:03</p>					
          <p class="b-audio-player__sound">						
            <span class="b-audio-player__mute">							
              <span class="icon-svg icon-svg--speaker ">	
                <svg class="icon-svg__svg" xmlns:xlink="http://www.w3.org/1999/xlink">		
                  <use xlink:href="https://www.irozhlas.cz/sites/all/themes/custom/irozhlas/img/bg/icons-svg.svg#icon-speaker" x="0" y="0" width="100%" height="100%">
                  </use>	
                </svg>
              </span>						
            </span>						
            <span class="b-audio-player__sound-bar">							
              <span class="icon-svg icon-svg--audio-player-dots ">	
                <svg class="icon-svg__svg" xmlns:xlink="http://www.w3.org/1999/xlink">		
                  <use xlink:href="https://www.irozhlas.cz/sites/all/themes/custom/irozhlas/img/bg/icons-svg.svg#icon-audio-player-dots" x="0" y="0" width="100%" height="100%">
                  </use>	
                </svg>
              </span>							
              <span class="b-audio-player__sound-progress" style="width: 100%;">								
                <span class="icon-svg icon-svg--audio-player-dots ">	
                  <svg class="icon-svg__svg" xmlns:xlink="http://www.w3.org/1999/xlink">		
                    <use xlink:href="https://www.irozhlas.cz/sites/all/themes/custom/irozhlas/img/bg/icons-svg.svg#icon-audio-player-dots" x="0" y="0" width="100%" height="100%">
                    </use>	
                  </svg>
                </span>							
              </span>						
            </span>					
          </p>					
          <div class="b-audio-player__bar">						
            <div class="b-audio-player__progress"></div>					
          </div>				
        </div>	
      </div>		
    </div>
	<br>


## Aktuální dění okolo koronaviru:

<!--[[ZPRAVY_LIVEREPORT:61920]]-->