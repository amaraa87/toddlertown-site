# toddlertown-site

Public web pages for the **Toddler Town Game** iOS app (iPhone + iPad, Kids category,
ages 5 and under): landing page, privacy policy and support, the URLs App Store Connect
requires. Published to GitHub Pages by `.github/workflows/pages.yml` on every push to `main`.

- Landing: https://amaraa87.github.io/toddlertown-site/
- Privacy policy: https://amaraa87.github.io/toddlertown-site/privacy/
- Support: https://amaraa87.github.io/toddlertown-site/support/

Plain HTML and one stylesheet (`assets/style.css`). No JavaScript, no web fonts, no
cookies, no trackers. Light and dark follow the system. Links are relative, so the site
works under the `/toddlertown-site/` base path or a custom domain.

## Keep in sync

The privacy policy must match what the 1.0 build actually does, the App Privacy answers in
App Store Connect ("Data Not Collected") and `PrivacyInfo.xcprivacy`. When one changes,
update the others. The policy describes the 1.0 build (town v2 + v3) and is only true once:

1. `ProjectSettings.asset` `submitAnalytics` is 0 ("Disable HW Statistics" checked). Today it
   is 1, which sends Unity hardware statistics from the player.
2. A network-monitor run (Little Snitch / mitmproxy) on the real 1.0 build shows no traffic.

Support page "How to play" lists v3 features (coins, vending machine, bakery, moving cars,
police car, fence hop, run). If any of them is cut from 1.0, remove it here too. Never list
unbuilt features (missions, Setsgoo, stickers, music/voice, saved progress, settings).

Credits name Meshy unconditionally, which also covers the CC BY 4.0 attribution needed if
any generation was made on Meshy's free plan. The App Store button links to
`apps.apple.com/app/id6821753444`, which works once the app is live.
