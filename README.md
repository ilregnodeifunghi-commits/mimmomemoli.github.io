HTML
<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Achillea tenorei Grande - Flora Digitalis</title>
    <style>
        /* STILI GENERALI (RESET E COLORI) */
        * { box-sizing: border-box; margin: 0; padding: 0; }
        body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; line-height: 1.6; color: #333; background-color: #f4f7f5; padding-bottom: 60px; }
        .container { max-width: 1100px; margin: 0 auto; padding: 20px; }
        
        /* HEADER / INTESTAZIONE */
        header { background-color: #2c5e3b; color: white; padding: 30px 20px; text-align: center; border-radius: 8px; margin-bottom: 25px; box-shadow: 0 4px 6px rgba(0,0,0,0.1); }
        header h1 { font-style: italic; font-size: 2.2rem; margin-bottom: 5px; }
        header .sub-title { font-size: 1.1rem; opacity: 0.9; font-weight: bold; }
        header .family { font-size: 0.95rem; text-transform: uppercase; letter-spacing: 1px; margin-top: 5px; opacity: 0.8; }

        /* STRUTTURA A DUE COLONNE (GALLERIA E TESTI) */
        .main-grid { display: grid; grid-template-columns: 1fr; gap: 25px; }
        @media (min-width: 850px) { .main-grid { grid-template-columns: 450px 1fr; } }

        /* COLONNA SINISTRA: GALLERIA BOTANICA SEZIONATA */
        .botanical-gallery { background: white; padding: 15px; border-radius: 8px; border: 1px solid #e0e6e2; box-shadow: 0 2px 4px rgba(0,0,0,0.05); height: fit-content; }
        .gallery-title { font-size: 1.1rem; color: #2c5e3b; font-weight: bold; margin-bottom: 12px; border-bottom: 2px solid #2c5e3b; padding-bottom: 5px; }
        .photo-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 10px; }
        .photo-card { background: #f9fbf9; border: 1px solid #d0dad2; border-radius: 6px; overflow: hidden; text-align: center; font-size: 0.85rem; font-weight: bold; color: #555; }
        .photo-box { height: 140px; background-color: #e2ebe4; display: flex; align-items: center; justify-content: center; color: #8fa393; font-style: italic; font-weight: normal; border-bottom: 1px solid #d0dad2; position: relative; }
        .photo-card span { display: block; padding: 6px 4px; background: white; }
        /* Il riquadro della pianta intera occupa due colonne per importanza */
        .photo-card.full-plant { grid-column: span 2; }
        .photo-card.full-plant .photo-box { height: 220px; }

        /* COLONNA DESTRA: SCHEDA SCHEMATICA DATI */
        .botanical-info { background: white; padding: 25px; border-radius: 8px; border: 1px solid #e0e6e2; box-shadow: 0 2px 4px rgba(0,0,0,0.05); }
        .section-block { margin-bottom: 25px; }
        .section-block:last-child { margin-bottom: 0; }
        .section-block h2 { color: #2c5e3b; font-size: 1.3rem; margin-bottom: 10px; border-bottom: 1px solid #d0dad2; padding-bottom: 4px; display: flex; align-items: center; }
        .section-block h2::before { content: "🌿"; margin-right: 8px; font-size: 1.1rem; }
        
        /* Liste ed elenchi */
        ul { list-style-type: none; }
        li { margin-bottom: 8px; padding-left: 15px; position: relative; }
        li::before { content: "•"; color: #2c5e3b; font-weight: bold; font-size: 1.2rem; position: absolute; left: 0; top: -2px; }
        strong { color: #111; }
        p { margin-bottom: 12px; text-align: justify; }

        /* Badge evidenziati */
        .badge-list { display: flex; flex-wrap: wrap; gap: 8px; margin-top: 10px; }
        .badge { background: #e2ebe4; color: #2c5e3b; padding: 4px 10px; border-radius: 4px; font-size: 0.85rem; font-weight: bold; border: 1px solid #cbdcd0; }
        .badge.alert { background: #fff1f1; color: #c92a2a; border-color: #ffc9c9; }
    </style>
</head>
<body>

    <div class="container">
        
        <!-- HEADER DELLA PIANTA -->
        <header>
            <h1>Achillea tenorei Grande</h1>
            <div class="sub-title">Nome comune: Achillea di Tenore, Millefoglio di Tenore</div>
            <div class="family">Famiglia: Asteraceae (Compositae)</div>
        </header>

        <!-- CONTENUTO PRINCIPALE -->
        <div class="main-grid">
            
            <!-- SINISTRA: GALLERIA FOTOGRAFICA SEZIONATA -->
            <aside class="botanical-gallery">
                <div class="gallery-title">Galleria Fotografica Organizzata</div>
                <div class="photo-grid">
                    
                    <!-- 1. Pianta Intera -->
                    <div class="photo-card full-plant">
                        <div class="photo-box">[ Inserisci Foto: Pianta Intera / Portamento ]</div>
                        <span>Pianta Intera / Portamento</span>
                    </div>
                    
                    <!-- 2. Fusto e Rami -->
                    <div class="photo-card">
                        <div class="photo-box">[ Foto: Fusto e Rami ]</div>
                        <span>Fusto e Rami</span>
                    </div>
                    
                    <!-- 3. Fogliame -->
                    <div class="photo-card">
                        <div class="photo-box">[ Foto: Fogliame ]</div>
                        <span>Fogliame</span>
                    </div>
                    
                    <!-- 4. Fiori -->
                    <div class="photo-card">
                        <div class="photo-box">[ Foto: Fiori / Infiorescenza ]</div>
                        <span>Fiori & Infiorescenza</span>
                    </div>
                    
                    <!-- 5. Frutti -->
                    <div class="photo-card">
                        <div class="photo-box">[ Foto: Frutti / Semi ]</div>
                        <span>Frutti & Semi</span>
                    </div>
                    
                    <!-- 6. Apparato Radicale -->
                    <div class="photo-card full-plant">
                        <div class="photo-box">[ Foto: Apparato Radicale / Rizoma ]</div>
                        <span>Apparato Radicale / Rizoma</span>
                    </div>

                </div>
            </aside>

            <!-- DESTRA: SCHEDA SCIENTIFICA COMPLETA -->
            <main class="botanical-info">
                
                <div class="section-block">
                    <h2>Inquadramento Tassonomico</h2>
                    <p>La <strong>Achillea tenorei Grande</strong> è un'entità botanica di straordinario valore scientifico, espressione dell'endemismo d'alta quota della penisola italiana. Dal punto di vista della moderna sistematica vegetale, questa entità è strettamente correlata al polimorfo aggregato di <strong>Achillea barrelieri (Ten.) Sch.Bip.</strong>, del quale rappresenta un sinonimo o una razza geografica altomontana.</p>
                    <div class="badge-list">
                        <div class="badge">Ploidia: Diploide</div>
                        <div class="badge">Genere: Achillea</div>
                        <div class="badge">Specie: A. tenorei</div>
                    </div>
                </div>

                <div class="section-block">
                    <h2>Caratteristiche Generali e Distintive</h2>
                    <ul>
                        <li><strong>Tipo di pianta:</strong> Erbacea perenne, emicrittofita scaposa.</li>
                        <li><strong>Pianta e Portamento:</strong> Sviluppa fusti fioriferi eretti o ascendenti, rigidetti, alti mediamente tra <strong>15 e 40 cm</strong>. I fusti sono cilindrici, debolmente striati e provvisti di una fine pubescenza.</li>
                        <li><strong>Foglie:</strong> Alterne lungo il fusto, mentre alla base formano dense rosette svernanti. La lamina ha un profilo da lineare a strettamente lanceolato ed è <strong>pennatosetta</strong>. I segmenti sono brevi, acuti e ordinati, di un colore verde vivo.</li>
                        <li><strong>Fiori:</strong> Infiorescenza terminale a corimbo composto, lasso. Capolini di 5-7 mm di diametro. I fiori ligulati esterni (generalmente 5) sono di colore <strong>bianco-candido</strong>, mentre i fiori tubulosi centrali sono piccolissimi e di colore <strong>giallo-crema</strong>.</li>
                        <li><strong>Periodo di fioritura:</strong> Fiorisce nel cuore dell'estate, tra <strong>luglio e agosto</strong>.</li>
                        <li><strong>Frutto:</strong> Achenio oblungo, compresso e liscio, privo di pappo.</li>
                    </ul>
                </div>

                <div class="section-block">
                    <h2>Origine, Corologia e Habitat</h2>
                    <ul>
                        <li><strong>Origine:</strong> <strong>Endemica italiana</strong> (esclusiva del territorio italiano).</li>
                        <li><strong>Corologia:</strong> Endemica Appenninica.</li>
                        <li><strong>Habitat d'elezione:</strong> Specie eliofila e orofila. Vegeta nella fascia montana superiore, subalpina e alpina, tra <strong>1200 e 2200 m s.l.m.</strong> Si trova su <strong>ghiaioni instabili, ravaneti, macereti, pietraie, pascoli rasi e fessure delle rocce calcaree</strong>. Esige suoli primitivi e perfettamente drenati.</li>
                    </ul>
                </div>

                <div class="section-block">
                    <h2>Proprietà ed Utilizzi</h2>
                    <ul>
                        <li><strong>Officinali:</strong> Uso tradizionale locale. Possiede proprietà <strong>vulnerarie (cicatrizzanti), toniche e digestive</strong> analoghe alle altre achillee montane; storicamente usata dai pastori per infusi d'alta quota.</li>
                        <li><strong>Alimentari:</strong> Nessun uso significativo a causa della consistenza coriacea e del sapore marcatamente amaro.</li>
                        <li><strong>Ornamentali:</strong> Interessante potenziale per il giardinaggio alpino ed ecologico (rock gardens, aiuole alpine e muretti a secco). Mostra ottima resistenza al freddo e alla siccità (Xerogardening).</li>
                        <li><strong>Tossicità:</strong> Generalmente non tossica. Può causare <strong>dermatiti allergiche da contatto</strong> in soggetti particolarmente sensibili alle Asteraceae a causa dei lattoni sesquiterpenici. Sconsigliata in gravidanza o con farmaci anticoagulanti.</li>
                        <li><strong>Ecologici:</strong> Svolge un ruolo cruciale come <strong>pianta pioniera</strong> per la stabilizzazione dei ghiaioni montani. I fiori sono un'importante fonte di nettare per insetti d'alta quota.</li>
                    </ul>
                </div>

                <div class="section-block">
                    <h2>Distribuzione in Italia e Protezione</h2>
                    <p>La specie è autoctona ed endemica della <strong>catena appenninica centrale e meridionale</strong>. Le sue popolazioni si concentrano sui massicci montuosi di <strong>Abruzzo, Molise, Lazio, Campania e Basilicata</strong>.</p>
                    <div class="badge-list">
                        <div class="badge">Areale: Frammentato / Ristretto</div>
                        <div class="badge alert">Protezione: Divieto di raccolta nei Parchi Nazionali</div>
                    </div>
                </div>

            </main>
        </div>
    </div>

</body>
</
   
    
