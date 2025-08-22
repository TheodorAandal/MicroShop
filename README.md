MicroShop – Microservices e-handelsplattform
🛠 Om prosjektet

ShopEasy er et microservices-prosjekt bygget med .NET 8, designet for å demonstrere moderne backend-arkitektur og cloud deployment.
Prosjektet består av tre microservices:

ProductService – håndterer produkter (CRUD).

OrderService – håndterer bestillinger.

NotificationService – sender notifikasjoner (simulert).

Prosjektet kan kjøre lokalt med Docker eller deployes til Azure Kubernetes Service (AKS).

⚡ Teknologier brukt

.NET 8 / ASP.NET Core Web API

Entity Framework Core med SQLite (lokalt)

Docker & Docker Compose

Azure: AKS, Container Registry, SQL Database, Key Vault, Application Insights

Git & GitHub for versjonskontroll

🚀 Komme i gang – lokalt
1. Klon repo
git clone https://github.com/<brukernavn>/ShopEasy.git
cd ShopEasy

2. Bygg og kjør med Docker Compose
docker-compose up --build


ProductService: http://localhost:5000/api/products

OrderService: http://localhost:5001/api/orders

NotificationService: logger meldinger i konsollen

3. Test API-endepunkter

Bruk Postman eller curl til å teste GET/POST på ProductService og OrderService.

🔧 Arkitektur

Microservices med egne databaser

API Gateway (YARP/Ocelot) samler tjenester til én inngang (valgfritt)

Event-driven kommunikasjon via NotificationService

Logging & observability med Serilog og Azure Application Insights

💡 Fremtidige forbedringer

Legge til Blazor WebAssembly frontend for handlekurv

Integrasjon med Azure Service Bus for event-driven kommunikasjon

CI/CD med GitHub Actions for automatisk deploy til AKS
