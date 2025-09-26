# ReVanced Magisk Module
[![CI](https://github.com/j-hc/revanced-magisk-module/actions/workflows/ci.yml/badge.svg?event=schedule)](https://github.com/j-hc/revanced-magisk-module/actions/workflows/ci.yml)

Compilatore App Revanced 

Scarica l'ultima [versione CI](https://github.com/j-hc/revanced-magisk-module/releases).

Utilizza [**zygisk-detach**](https://github.com/j-hc/zygisk-detach) per scollegare Youtube e YT Music dal Play Store se stai usando il modulo KSU.

<details><summary><big>Caratteristiche</big></summary>
<ul>
 <li>Supporta tutte le app ReVanced e <a href="https://github.com/inotia00/revanced-patches">ReVanced Extended</a> presenti e future</li>
 <li> Può creare moduli KSU e APK non-root</li>
 <li> Aggiornato quotidianamente con le ultime versioni di app e patch</li>
 <li> Ottimizza le dimensioni di APK e moduli</li>
 <li> Moduli</li>
    <ul>
     <li> Ricompila gli odex invalidati per un utilizzo più rapido</li>
     <li> Riceve gli aggiornamenti dal manager di KSU</li>
     <li> Non compromette SafetyNet né attiva i rilevamenti di root</li>
     <li> Gestisce l'installazione della versione corretta dell'app stock e tutto il resto</li>
     <li> Supporta Magisk e KernelSU</li>
    </ul>
</ul>
Nota che il <a href="../../actions/workflows/ci.yml">CI workflow</a> è programmato per creare i moduli e gli APK ogni giorno tramite GitHub Actions se c'è una modifica nelle patch di ReVanced. Potresti volerlo disabilitare.
</details>

## Per includere/escludere patch o patchare altre app

 * Use the repo as a [template](https://github.com/new?template_name=revanced-magisk-module&template_owner=j-hc)
 * Personalizza [`config.toml`](./config.toml) usando [rvmm-config-gen](https://j-hc.github.io/rvmm-config-gen/)
 * Esegui il [workflow](../../actions/workflows/build.yml)
 * Scarica i moduli e gli APK dalla pagina delle [release](../../releases)

vedi anche qua [`CONFIG.md`](./CONFIG.md)

## Compilazione in locale
### Termux
```console
bash <(curl -sSf https://raw.githubusercontent.com/j-hc/revanced-magisk-module/main/build-termux.sh)
```

### Desktop
```console
$ git clone https://github.com/j-hc/revanced-magisk-module
$ cd revanced-magisk-module
$ ./build.sh
```
