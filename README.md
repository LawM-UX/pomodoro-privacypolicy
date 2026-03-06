<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Privacy Policy — Focus Flow</title>
  <style>
    :root {
      --bg:        #0f0f12;
      --surface:   #1a1a22;
      --border:    #2a2a38;
      --accent:    #ff7a3c;
      --text:      #e8e8f0;
      --muted:     #8888aa;
      --radius:    14px;
    }

    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
                   Helvetica, Arial, sans-serif;
      background: var(--bg);
      color: var(--text);
      line-height: 1.7;
      padding: 0 16px 80px;
    }

    /* ── Lang toggle ── */
    .lang-bar {
      position: sticky;
      top: 0;
      z-index: 10;
      background: var(--bg);
      border-bottom: 1px solid var(--border);
      display: flex;
      justify-content: flex-end;
      gap: 8px;
      padding: 10px 16px;
    }
    .lang-btn {
      background: var(--surface);
      border: 1px solid var(--border);
      color: var(--muted);
      border-radius: 20px;
      padding: 4px 14px;
      font-size: 13px;
      cursor: pointer;
      transition: all .2s;
    }
    .lang-btn.active {
      background: var(--accent);
      border-color: var(--accent);
      color: #fff;
    }

    /* ── Layout ── */
    .container { max-width: 760px; margin: 0 auto; }

    /* ── Hero ── */
    .hero {
      text-align: center;
      padding: 56px 0 40px;
    }
    .hero-icon {
      width: 80px; height: 80px;
      border-radius: 22px;
      background: linear-gradient(135deg, #ff7a3c, #ff3c6e);
      display: inline-flex;
      align-items: center;
      justify-content: center;
      font-size: 38px;
      margin-bottom: 20px;
      box-shadow: 0 8px 32px rgba(255,122,60,.35);
    }
    .hero h1 {
      font-size: clamp(26px, 5vw, 36px);
      font-weight: 700;
      letter-spacing: -.5px;
    }
    .hero .subtitle {
      color: var(--muted);
      font-size: 15px;
      margin-top: 8px;
    }
    .updated-badge {
      display: inline-block;
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: 20px;
      padding: 4px 14px;
      font-size: 12px;
      color: var(--muted);
      margin-top: 16px;
    }

    /* ── Cards ── */
    .card {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 28px;
      margin-bottom: 16px;
    }
    .card-header {
      display: flex;
      align-items: center;
      gap: 12px;
      margin-bottom: 16px;
    }
    .card-icon {
      width: 38px; height: 38px;
      border-radius: 10px;
      background: rgba(255,122,60,.12);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 18px;
      flex-shrink: 0;
    }
    .card h2 {
      font-size: 17px;
      font-weight: 700;
    }
    .card p { color: var(--muted); font-size: 15px; }
    .card p + p { margin-top: 10px; }

    /* ── List ── */
    ul.check {
      list-style: none;
      display: flex;
      flex-direction: column;
      gap: 8px;
      margin-top: 12px;
    }
    ul.check li {
      display: flex;
      align-items: flex-start;
      gap: 10px;
      font-size: 15px;
      color: var(--muted);
    }
    ul.check li::before {
      content: "✓";
      color: #34d058;
      font-weight: 700;
      flex-shrink: 0;
      margin-top: 2px;
    }

    /* ── Highlight box ── */
    .highlight {
      background: rgba(255,122,60,.08);
      border-left: 3px solid var(--accent);
      border-radius: 0 8px 8px 0;
      padding: 14px 18px;
      font-size: 14px;
      color: var(--text);
      margin-top: 14px;
    }

    /* ── External link ── */
    a { color: var(--accent); text-decoration: none; }
    a:hover { text-decoration: underline; }

    /* ── Footer ── */
    footer {
      text-align: center;
      color: var(--muted);
      font-size: 13px;
      padding-top: 40px;
      border-top: 1px solid var(--border);
      margin-top: 40px;
    }

    /* ── Language switching ── */
    .lang-en, .lang-fr { display: none; }
    body.show-en .lang-en { display: block; }
    body.show-fr .lang-fr { display: block; }

    /* show english by default */
    body:not(.show-fr) .lang-en { display: block; }
    body.show-fr      .lang-en { display: none; }
  </style>
</head>
<body>

<!-- ── Language bar ── -->
<div class="lang-bar">
  <button class="lang-btn active" onclick="setLang('en', this)">🇬🇧 English</button>
  <button class="lang-btn"        onclick="setLang('fr', this)">🇫🇷 Français</button>
</div>

<div class="container">

  <!-- ══ HERO ══ -->
  <div class="hero">
    <div class="hero-icon">🍅</div>
    <h1>Focus Flow — Privacy Policy</h1>
    <p class="subtitle lang-en">Your focus. Your data. Your device.</p>
    <p class="subtitle lang-fr">Votre concentration. Vos données. Votre appareil.</p>
    <span class="updated-badge lang-en">Last updated: March 2026</span>
    <span class="updated-badge lang-fr">Dernière mise à jour : mars 2026</span>
  </div>

  <!-- ══ 1. OVERVIEW ══ -->
  <div class="card">
    <div class="card-header">
      <div class="card-icon">👁️</div>
      <h2 class="lang-en">Overview</h2>
      <h2 class="lang-fr">Vue d'ensemble</h2>
    </div>

    <div class="lang-en">
      <p>Focus Flow ("we", "our", "the app") is a Pomodoro productivity timer for iOS developed by an independent developer. We are committed to protecting your privacy.</p>
      <p>This Privacy Policy describes what information the app accesses, how it is used, and your rights regarding that information.</p>
      <div class="highlight">
        <strong>Short version:</strong> Focus Flow does not collect, store, or sell your personal data. All timer settings and preferences are saved <em>locally on your device only</em>.
      </div>
    </div>
    <div class="lang-fr">
      <p>Focus Flow (« nous », « notre application ») est un minuteur de productivité Pomodoro pour iOS, développé par un développeur indépendant. Nous nous engageons à protéger votre vie privée.</p>
      <p>Cette politique de confidentialité décrit les informations auxquelles l'application accède, comment elles sont utilisées, et vos droits à cet égard.</p>
      <div class="highlight">
        <strong>Résumé :</strong> Focus Flow ne collecte, ne stocke, ni ne vend vos données personnelles. Tous vos réglages et préférences sont sauvegardés <em>uniquement en local sur votre appareil</em>.
      </div>
    </div>
  </div>

  <!-- ══ 2. DATA WE DO NOT COLLECT ══ -->
  <div class="card">
    <div class="card-header">
      <div class="card-icon">🔒</div>
      <h2 class="lang-en">Data We Do NOT Collect</h2>
      <h2 class="lang-fr">Données que nous ne collectons PAS</h2>
    </div>
    <ul class="check">
      <li class="lang-en">Your name, email address, or any personal identifiers</li>
      <li class="lang-fr">Votre nom, adresse e-mail ou tout identifiant personnel</li>
      <li class="lang-en">Your location or GPS data</li>
      <li class="lang-fr">Votre localisation ou données GPS</li>
      <li class="lang-en">Your contacts, photos, camera, or microphone</li>
      <li class="lang-fr">Vos contacts, photos, caméra ou microphone</li>
      <li class="lang-en">Your health or biometric data</li>
      <li class="lang-fr">Vos données de santé ou biométriques</li>
      <li class="lang-en">Your browsing history or usage behavior (beyond AdMob — see below)</li>
      <li class="lang-fr">Votre historique de navigation ou comportement d'utilisation (hors AdMob — voir ci-dessous)</li>
    </ul>
  </div>

  <!-- ══ 3. LOCAL DATA ══ -->
  <div class="card">
    <div class="card-header">
      <div class="card-icon">📱</div>
      <h2 class="lang-en">Data Stored Locally on Your Device</h2>
      <h2 class="lang-fr">Données stockées localement sur votre appareil</h2>
    </div>
    <div class="lang-en">
      <p>Focus Flow saves the following information <strong>exclusively on your device</strong> using Apple's <code>UserDefaults</code> (standard iOS local storage). This data never leaves your device and is never transmitted to our servers or any third party:</p>
    </div>
    <div class="lang-fr">
      <p>Focus Flow sauvegarde les informations suivantes <strong>exclusivement sur votre appareil</strong> via <code>UserDefaults</code> d'Apple (stockage local iOS standard). Ces données ne quittent jamais votre appareil et ne sont jamais transmises à nos serveurs ou à des tiers :</p>
    </div>
    <ul class="check" style="margin-top:14px;">
      <li class="lang-en">Timer durations (focus, short break, long break)</li>
      <li class="lang-fr">Durées du minuteur (concentration, pause courte, pause longue)</li>
      <li class="lang-en">Number of rounds per session</li>
      <li class="lang-fr">Nombre de tours par session</li>
      <li class="lang-en">Auto-start preferences</li>
      <li class="lang-fr">Préférences de démarrage automatique</li>
      <li class="lang-en">Sound and notification preferences</li>
      <li class="lang-fr">Préférences de son et de notifications</li>
      <li class="lang-en">In-app purchase status (ads removed)</li>
      <li class="lang-fr">Statut de l'achat intégré (publicités supprimées)</li>
    </ul>
  </div>

  <!-- ══ 4. ADVERTISING (ADMOB) ══ -->
  <div class="card">
    <div class="card-header">
      <div class="card-icon">📢</div>
      <h2 class="lang-en">Advertising — Google AdMob</h2>
      <h2 class="lang-fr">Publicité — Google AdMob</h2>
    </div>
    <div class="lang-en">
      <p>The free version of Focus Flow displays advertisements provided by <strong>Google AdMob</strong>. Google AdMob may collect and use certain data to serve personalised or non-personalised ads, which may include:</p>
      <ul class="check" style="margin-top:12px;">
        <li>Advertising identifiers (IDFA) — only if you grant App Tracking Transparency permission</li>
        <li>Device information (model, operating system version)</li>
        <li>IP address (used to infer approximate location for ad targeting)</li>
        <li>Ad interaction data (impressions, clicks)</li>
      </ul>
      <p style="margin-top:14px;">Google's data collection is governed by Google's Privacy Policy. You can review it at <a href="https://policies.google.com/privacy" target="_blank">policies.google.com/privacy</a>.</p>
      <p>You can opt out of personalised advertising at any time in <strong>iOS Settings → Privacy & Security → Apple Advertising</strong>, or by purchasing the <strong>Remove Ads</strong> upgrade inside the app.</p>
    </div>
    <div class="lang-fr">
      <p>La version gratuite de Focus Flow affiche des publicités fournies par <strong>Google AdMob</strong>. Google AdMob peut collecter et utiliser certaines données pour diffuser des annonces personnalisées ou non personnalisées, notamment :</p>
      <ul class="check" style="margin-top:12px;">
        <li>Identifiant publicitaire (IDFA) — uniquement si vous accordez l'autorisation App Tracking Transparency</li>
        <li>Informations sur l'appareil (modèle, version du système d'exploitation)</li>
        <li>Adresse IP (utilisée pour déduire une localisation approximative)</li>
        <li>Données d'interaction avec les annonces (impressions, clics)</li>
      </ul>
      <p style="margin-top:14px;">La collecte de données par Google est régie par la politique de confidentialité de Google, consultable sur <a href="https://policies.google.com/privacy" target="_blank">policies.google.com/privacy</a>.</p>
      <p>Vous pouvez désactiver la publicité personnalisée à tout moment dans <strong>Réglages iOS → Confidentialité et sécurité → Publicité Apple</strong>, ou en achetant la mise à niveau <strong>Supprimer les pubs</strong> dans l'application.</p>
    </div>
  </div>

  <!-- ══ 5. IN-APP PURCHASES ══ -->
  <div class="card">
    <div class="card-header">
      <div class="card-icon">💳</div>
      <h2 class="lang-en">In-App Purchases</h2>
      <h2 class="lang-fr">Achats intégrés</h2>
    </div>
    <div class="lang-en">
      <p>The "Remove Ads" purchase is processed entirely by <strong>Apple's App Store</strong> via StoreKit 2. We do not receive, process, or store any payment or financial information. All purchase transactions are handled solely by Apple.</p>
      <p>For questions about Apple's data handling for purchases, please refer to <a href="https://www.apple.com/legal/privacy/" target="_blank">Apple's Privacy Policy</a>.</p>
    </div>
    <div class="lang-fr">
      <p>L'achat « Supprimer les pubs » est entièrement traité par l'<strong>App Store d'Apple</strong> via StoreKit 2. Nous ne recevons, ne traitons, ni ne stockons aucune information de paiement ou financière. Toutes les transactions sont gérées exclusivement par Apple.</p>
      <p>Pour toute question sur la gestion des données d'achat par Apple, veuillez consulter la <a href="https://www.apple.com/legal/privacy/fr/" target="_blank">Politique de confidentialité d'Apple</a>.</p>
    </div>
  </div>

  <!-- ══ 6. NOTIFICATIONS ══ -->
  <div class="card">
    <div class="card-header">
      <div class="card-icon">🔔</div>
      <h2 class="lang-en">Notifications &amp; Live Activities</h2>
      <h2 class="lang-fr">Notifications et activités en direct</h2>
    </div>
    <div class="lang-en">
      <p>If you grant permission, Focus Flow uses Apple's <strong>UserNotifications</strong> framework to send local notifications when a Pomodoro phase ends. These notifications are generated entirely on your device and are not sent to or via any external server.</p>
      <p>Live Activities (lock screen widget / Dynamic Island) display your current timer state. This information is processed locally and is not transmitted externally.</p>
    </div>
    <div class="lang-fr">
      <p>Si vous accordez l'autorisation, Focus Flow utilise le framework <strong>UserNotifications</strong> d'Apple pour envoyer des notifications locales lorsqu'une phase Pomodoro se termine. Ces notifications sont générées entièrement sur votre appareil et ne transitent par aucun serveur externe.</p>
      <p>Les activités en direct (widget sur l'écran verrouillé / Dynamic Island) affichent l'état actuel de votre minuteur. Ces informations sont traitées localement et ne sont pas transmises à l'extérieur.</p>
    </div>
  </div>

  <!-- ══ 7. CHILDREN ══ -->
  <div class="card">
    <div class="card-header">
      <div class="card-icon">👶</div>
      <h2 class="lang-en">Children's Privacy</h2>
      <h2 class="lang-fr">Confidentialité des enfants</h2>
    </div>
    <div class="lang-en">
      <p>Focus Flow does not knowingly collect personal information from children under the age of 13. If you are a parent or guardian and believe your child has provided personal information, please contact us and we will take appropriate steps to remove such information.</p>
    </div>
    <div class="lang-fr">
      <p>Focus Flow ne collecte pas sciemment d'informations personnelles auprès d'enfants de moins de 13 ans. Si vous êtes parent ou tuteur et pensez que votre enfant a fourni des informations personnelles, veuillez nous contacter et nous prendrons les mesures appropriées pour supprimer ces informations.</p>
    </div>
  </div>

  <!-- ══ 8. YOUR RIGHTS ══ -->
  <div class="card">
    <div class="card-header">
      <div class="card-icon">⚖️</div>
      <h2 class="lang-en">Your Rights (GDPR / CCPA)</h2>
      <h2 class="lang-fr">Vos droits (RGPD / CCPA)</h2>
    </div>
    <div class="lang-en">
      <p>Since Focus Flow does not collect personal data beyond what AdMob may collect (described above), there is no personal data held by us to access, correct, or delete.</p>
      <p>For data collected by Google AdMob, you may exercise your rights directly with Google at <a href="https://myaccount.google.com/data-and-privacy" target="_blank">myaccount.google.com</a>.</p>
      <p>To delete all app data, simply delete Focus Flow from your device. All locally stored preferences will be permanently removed.</p>
    </div>
    <div class="lang-fr">
      <p>Puisque Focus Flow ne collecte pas de données personnelles au-delà de ce que peut collecter AdMob (décrit ci-dessus), il n'existe aucune donnée personnelle détenue par nous à accéder, corriger ou supprimer.</p>
      <p>Pour les données collectées par Google AdMob, vous pouvez exercer vos droits directement auprès de Google sur <a href="https://myaccount.google.com/data-and-privacy" target="_blank">myaccount.google.com</a>.</p>
      <p>Pour supprimer toutes les données de l'application, supprimez simplement Focus Flow de votre appareil. Toutes les préférences stockées localement seront définitivement effacées.</p>
    </div>
  </div>

  <!-- ══ 9. CHANGES ══ -->
  <div class="card">
    <div class="card-header">
      <div class="card-icon">📝</div>
      <h2 class="lang-en">Changes to This Policy</h2>
      <h2 class="lang-fr">Modifications de cette politique</h2>
    </div>
    <div class="lang-en">
      <p>We may update this Privacy Policy from time to time. Any changes will be posted on this page with an updated revision date. We encourage you to review this page periodically. Continued use of the app after changes constitutes acceptance of the updated policy.</p>
    </div>
    <div class="lang-fr">
      <p>Nous pouvons mettre à jour cette politique de confidentialité de temps en temps. Tout changement sera publié sur cette page avec une date de révision mise à jour. Nous vous encourageons à consulter cette page régulièrement. L'utilisation continue de l'application après des modifications constitue l'acceptation de la politique mise à jour.</p>
    </div>
  </div>

  <!-- ══ 10. CONTACT ══ -->
  <div class="card">
    <div class="card-header">
      <div class="card-icon">✉️</div>
      <h2 class="lang-en">Contact</h2>
      <h2 class="lang-fr">Contact</h2>
    </div>
    <div class="lang-en">
      <p>If you have any questions or concerns about this Privacy Policy, please contact us at:</p>
      <p><strong>Email:</strong> <a href="mailto:privacy@focusflow.app">privacy@focusflow.app</a></p>
      <p class="highlight">Replace the email above with your actual support/privacy contact email before publishing.</p>
    </div>
    <div class="lang-fr">
      <p>Si vous avez des questions ou des préoccupations concernant cette politique de confidentialité, veuillez nous contacter à :</p>
      <p><strong>E-mail :</strong> <a href="mailto:privacy@focusflow.app">privacy@focusflow.app</a></p>
      <p class="highlight">Remplacez l'e-mail ci-dessus par votre vrai e-mail de support/confidentialité avant de publier.</p>
    </div>
  </div>

  <!-- ══ FOOTER ══ -->
  <footer>
    <p>© 2026 Focus Flow. All rights reserved.</p>
    <p style="margin-top:6px;">
      <a href="https://www.apple.com/legal/privacy/" target="_blank">Apple Privacy Policy</a> ·
      <a href="https://policies.google.com/privacy" target="_blank">Google Privacy Policy</a>
    </p>
  </footer>

</div><!-- /container -->

<script>
  function setLang(lang, btn) {
    document.querySelectorAll('.lang-btn').forEach(b => b.classList.remove('active'));
    btn.classList.add('active');
    document.body.classList.remove('show-en', 'show-fr');
    document.body.classList.add('show-' + lang);
  }
</script>
</body>
</html>
