# Zásady ochrany osobních údajů - Saber

Jedná se o neoficiální překlad
[anglického originálu](https://github.com/adil192/saber/blob/main/privacy_policy.md).
Autor se vzdává veškeré zodpovědnosti za vzniklé nedorozumění, misinterpretace
či nepochopení založené na nepřesnostech či chybách v překladu. Tento překlad
slouží výhradně pro vytvoření představy o obsahu anglického originálu pro česky
mluvící uživatele, kteří nejsou schopni číst původní verzi. Pro přesné právní
výklady či právní spory by měl být využit výhradně původní zdroj. Autor překladu
dále nezaručuje, že bude tento soubor vycházet z aktuálního originálu. Jeho
obsah může být i výrazně opožděný.

Saber je aplikace vyvinutá Adilem Hanneym, která uživatelům usnadňuje
vytváření a organizaci ručně psaných poznámek.

Tyto zásady ochrany osobních údajů (anglický originál) se budou měnit, jak se bude
aplikace vyvíjet: na této stránce si můžete prohlédnout veškeré změny a sledovat
vývoj aplikace prostřednictvím
[diskuze věnované vývoji aplikace Saber](https://github.com/adil192/saber/discussions/1)
(anglicky) a záznamů o změnách na stránce
[Vydání](https://github.com/adil192/saber/releases) (anglicky).

## Jaká data aplikace využívá?

Aplikace usiluje o přístup k co nejmenšímu množství dat a používá princip nulové
důvěry ke cloudovému úložišti.

Uživatelská data, která aplikace používá, zahrnují:
- Poznámky (včetně obrázků a pozadí): Používána pro hlavní funkcionalitu aplikace
- Nastavení uvnitř aplikace: Používáno pro přizpůsobení aplikace uživatelským preferencím
- Přístupové údaje do online cloudové služby (dále jen "cloud") zahrnující URI serveru, uživatelské jméno a heslo: Používány k umožnění synchronizace mezi zařízeními
- Data využívaná třetími stranami (viz níže)

### Využití dat třetími stranami

Za účelem nabídnutí některých funkcí aplikace používá služby třetích stran.

#### Google AdMob

Některé verze aplikace podporují reklamy Google AdMob zahrnující reklamní síť společnosti Google
a dalších sítí splňující nařízení GDPR:
- Verze pro iOS dostupná na App Store
- Verze pro Android dostupná na Google Play Store
- Verze pro Android dostupná ze stránky [Vydání](https://github.com/adil192/saber/releases), která je součástí repozitáře na GitHubu

TODO: continue later

Note that the Android version available on F-Droid does not use Google AdMob or contain ads.

AdMob may collect data about you, including your device's advertising ID, IP address, and location. You can read more about [how Google uses data from apps that use their services](https://policies.google.com/technologies/partner-sites).

When you first open Saber, you will be asked to choose between personalized ads and non-personalized ads. You can change this at any time on the Settings page, or disable ads completely. 

## How is the cloud used?

The cloud is used to store and sync the user's notes and settings
between the user's devices but is not necessary for the application to function.

To use this feature, users need to make an account on a Nextcloud server
of their choice to use as a cloud service.
For users who don't want to choose a custom Nextcloud server,
the official Saber server — run by Adil Hanney — is hosted at
[nc.saber.adil.hanney.org](https://nc.saber.adil.hanney.org).

To maintain privacy, all notes are encrypted before being sent to the cloud.
A randomly generated key is used to encrypt the notes.
This key and password are stored on the user's device in secure storage,
and an encrypted form of the key is uploaded to the cloud.

### My notes are private, right?

With any cloud storage, the server owners can see and read any files you upload.
This is why Saber encrypts your notes before uploading them to the cloud,
so they're unreadable to the server owner.

### So what data can the server owners see?

- All information provided during the sign-up process, including but not limited to your username and email address.
- Information about any device that connects to the server, including but not limited to the device's operating system, browser, and IP address.
- An encrypted (scrambled) form of your notes. However, the server owner can see:
  - The size of each note.
  - The number of notes you have.
  - The last time you edited a note, when it was created, and when you last synced.
- An encrypted (scrambled) form of your encryption key. This is required to enable cross-device syncing.
- Nextcloud is general-purpose software, so the server owner can see any other files you upload
  to the server and information you provide outside of Saber.

## “Talk is cheap. Show me the code.”

The source code is free and open to the public under the
[GPLv3 license](https://github.com/adil192/saber/blob/main/LICENSE.md)
and is available on [GitHub](https://github.com/adil192/saber).

## How can I delete my data?

How you can delete your data will vary based on which cloud provider you use.
1. If you don't use a cloud provider, your data is only stored on your device.
  If you delete the app, your data will be deleted with it. Desktop users will
  also need to delete the `Saber` folder in your Documents folder.
2. If you use the default cloud provider, you can head to the
  [account deletion page](https://nc.saber.adil.hanney.org/index.php/settings/user/drop_account)
  by going to Settings then "Delete account". You'll get an email with a link to confirm
  the deletion of your account. Once you click the link, your account will be deleted after
  a 1 week grace period. If you change your mind, contact me at
  [adilhanney@disroot.org](mailto:adilhanney@disroot.org) and I'll cancel the deletion.
3. If you use a third-party Nextcloud server, there may be a "Delete account" option in the Settings.
  If not, you may need to contact the server administrator to delete your account.
  You should see the server's privacy policy for more information.

## Privacy point of contact

This application is developed by Adil Hanney.
You can contact me at [adilhanney@disroot.org](mailto:adilhanney@disroot.org) for any enquiries,
or [create an issue](https://github.com/adil192/saber/issues/new/choose)
on this repo (requires a GitHub account).
