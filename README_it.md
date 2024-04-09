<!--
N.B.: Questo README è stato automaticamente generato da <https://github.com/YunoHost/apps/tree/master/tools/readme_generator>
NON DEVE essere modificato manualmente.
-->

# Scrutiny per YunoHost

[![Livello di integrazione](https://dash.yunohost.org/integration/scrutiny.svg)](https://dash.yunohost.org/appci/app/scrutiny) ![Stato di funzionamento](https://ci-apps.yunohost.org/ci/badges/scrutiny.status.svg) ![Stato di manutenzione](https://ci-apps.yunohost.org/ci/badges/scrutiny.maintain.svg)

[![Installa Scrutiny con YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=scrutiny)

*[Leggi questo README in altre lingue.](./ALL_README.md)*

> *Questo pacchetto ti permette di installare Scrutiny su un server YunoHost in modo semplice e veloce.*  
> *Se non hai YunoHost, consulta [la guida](https://yunohost.org/install) per imparare a installarlo.*

## Panoramica

**Scrutiny is a Hard Drive Health Dashboard & Monitoring solution, merging manufacturer provided S.M.A.R.T metrics with real-world failure rates.**

> NOTE: Scrutiny is a Work-in-Progress and still has some rough edges.

### Features

Scrutiny is a simple but focused application, with a couple of core features:

- Web UI Dashboard - focused on Critical metrics
- `smartd` integration (no re-inventing the wheel)
- Auto-detection of all connected hard-drives
- S.M.A.R.T metric tracking for historical trends
- Customized thresholds using real world failure rates
- Temperature tracking
- Provided as an all-in-one Docker image (but can be installed manually)
- Configurable Alerting/Notifications via Webhooks
- (Future) Hard Drive performance testing & tracking


**Versione pubblicata:** 0.8.0~ynh1

## Screenshot

![Screenshot di Scrutiny](./doc/screenshots/dashboard.png)

## Documentazione e risorse

- Documentazione ufficiale per gli amministratori: <https://github.com/AnalogJ/scrutiny/tree/master/docs>
- Repository upstream del codice dell’app: <https://github.com/AnalogJ/scrutiny>
- Store di YunoHost: <https://apps.yunohost.org/app/scrutiny>
- Segnala un problema: <https://github.com/YunoHost-Apps/scrutiny_ynh/issues>

## Informazioni per sviluppatori

Si prega di inviare la tua pull request alla [branch di `testing`](https://github.com/YunoHost-Apps/scrutiny_ynh/tree/testing).

Per provare la branch di `testing`, si prega di procedere in questo modo:

```bash
sudo yunohost app install https://github.com/YunoHost-Apps/scrutiny_ynh/tree/testing --debug
o
sudo yunohost app upgrade scrutiny -u https://github.com/YunoHost-Apps/scrutiny_ynh/tree/testing --debug
```

**Maggiori informazioni riguardo il pacchetto di quest’app:** <https://yunohost.org/packaging_apps>
