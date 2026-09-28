# Stuekontroll

Mobiltilpasset PWA for TV og lys via Home Assistant + Broadlink RM4 Mini.

## TV-kommandoer
Appen bruker device `tv` og kommandoene: `power`, `volume_up`, `volume_down`, `mute`, `up`, `down`, `left`, `right`, `ok`, `back`, `exit`, `source`, `settings`.

## Oppsett
Åpne fanen **Oppsett** og legg inn Home Assistant URL, Long-Lived Access Token og remote entity-id. Opplysningene lagres lokalt i nettleseren.

> Merk: Direkte nettleserkall til Home Assistant kan kreve at Home Assistant tillater origin/CORS for domenet appen kjører på. Ikke legg access token i kildekoden eller commit det til GitHub.

## Telys
Lysfanen forventer script-entitetene `script.telys_on_alle`, `script.telys_off_alle`, `script.telys_flame` og `script.telys_static`. Endre navn i `app.js` hvis entity-id-ene i Home Assistant er annerledes.
