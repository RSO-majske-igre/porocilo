# Sistem za organiziranje prijav na dogodke v okviru Majskih iger

__Matjaž Bizjak, Jakob Marušič__

__Računalniške storitve v oblaku, 2022/23__

## Opis projekta

Sistem je namenjen organizacijski ekipi Majskih iger. Majske igre so tritedenski športno, kulturno, zabavni dogodek. Osrednji element dogodkov je meddomsko športno tekmovanje v več kot 40 športnimi disciplinami, v katerih tekmujejo stanovalci Študentskih domov Ljubljana.

Sistem za organizacijo prijav na dogodke omogoča organizatorjem kreiranje dogodkov in sodelujočih ter kreiranje prijav na posamezne dogodke. Hkrati se ob prijavi generira račun za vsakega izmed udeležencev v zunanji storitvi Stripe, poleg tega vsak udeleženec dogodka prejme potrditev vpisa na elektornski naslov.

## Ogrodje in razvojno okolje

Za razvoj zalednih mikrostoritev je bilo uporabljeno ogrodje __Spring Boot__. Za shranjevanje podatkov mikrostoritve uporabljajo podatkovno bazo MariaDB, do katere dostopajo preko vmesnika JPA in Hibernate.

Za razvoj čelnega dela sistema je bilo uporabljeno ogrodje __Angular__, ki znotraj lastnega vmesnika uporablja nginx spletni strežnik. Pri razvoju je bilo uporabljeno tudi ogrodje Bulma za hitro prototipiranje stilov.

// TODO: Matjaž

Pri razvoju čelnih in zalednih mikrostoritev je bilo uporabljeno razvojno okolje __IntelliJ__.

## Povezave do repozitorijev

### Zaledne storitve

| Ime storitve | Tip storitve | GitHub (izvorna koda) | DockerHub |
| ------------ | ------------ | --------------------- | --------- |
| Events backend | Spring Boot mikrostoritev | [https://github.com/RSO-majske-igre/events_backend](https://github.com/RSO-majske-igre/events_backend) | [https://hub.docker.com/r/bizjak3/events_backend](https://hub.docker.com/r/bizjak3/events_backend) |
| Email backend | Spring Boot mikrostoritev | [https://github.com/RSO-majske-igre/email_backend](https://github.com/RSO-majske-igre/email_backend) | [https://hub.docker.com/r/bizjak3/email_backend](https://hub.docker.com/r/bizjak3/email_backend) |
| Payments backend | Spring Boot mikrostoritev | [https://github.com/RSO-majske-igre/payment_backend](https://github.com/RSO-majske-igre/payment_backend) | [https://hub.docker.com/r/bizjak3/payments_backend](https://hub.docker.com/r/bizjak3/payments_backend) |
| Participant backend | Spring Boot mikrostoritev | [https://github.com/RSO-majske-igre/users_backend](https://github.com/RSO-majske-igre/users_backend) | [https://hub.docker.com/r/bizjak3/users_backend](https://hub.docker.com/r/bizjak3/users_backend)

### Čelne storitve

| Ime storitve | Tip storitve | GitHub (izvorna koda) | DockerHub |
| ------------ | ------------ | --------------------- | --------- |
| Angular aplikacija | spletna stran | [https://github.com/RSO-majske-igre/frontend](https://github.com/RSO-majske-igre/frontend) | [https://hub.docker.com/r/bizjak3/frontend](https://hub.docker.com/r/bizjak3/frontend) |

### Repozitoriji konfiguracije

| Ime storitve | Tip storitve | GitHub (izvorna koda) |
| ------------ | ------------ | --------------------- |
| k8s | Konfiguracija Kubernetes | [https://github.com/RSO-majske-igre/k8s](https://github.com/RSO-majske-igre/k8s) |
| spring_cloud | Konfiguracija Spring Cloud | [https://github.com/RSO-majske-igre/spring_cloud](https://github.com/RSO-majske-igre/spring_cloud) |

## Shema arhitekture in iterakcij

## Funkcionalnosti sistema
Seznam funkcionalnosti, ki jih mikrostoritve implementirajo (za vsako mikrostoritev naštejte funkcionalnosti, ki jih implementira). 

## Implementirani primeri uporabe
Seznam primerov uporabe, ki ste jih implementirali.

## Namestitev na Kubernetes
Kratek opis namestitve na Kubernetes (navedite izbranega ponudnika oblačnih storitev, naslov URL, na katerem je vaša aplikacija dostopna, in vključutev Ingressa).

## Uporaba konfiguracij
Kratek opis uporabe različnih virov konfiguracije v vaših rešitvah.

## Kontrole zdravja in metrike
Seznam implementiranih kontrol zdravja in metrik.

## Zunanji API-ji
Kratek opis uporabe zunanjih API-jev v vaših rešitvah.

## OpenApi dokumentacija
Kratek opis dokumentiranja storitev z uporabo OpenAPI.

## Centralizirano beleženje dnevnikov
Kratek opis centraliziranega beleženja dnevnikov v vaši aplikaciji.

## Izolacija in toleranca napak
Kratek opis demonstracije za izolacijo in toleranco napak, ki ste jo pripravili za vašo aplikacijo.