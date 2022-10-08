
Video :
"Getting started with GraphQL and Blazor" 

https://www.youtube.com/watch?v=-oq7YEciouM&t=1296s 


opprett en ny mappe under feks c:\src\somedemo
kjør : 
dotnet new blazorwasm --force 

legg til StrawberryShake.Blazor pakke (preview 65 ser ut til å virke best med dotnet tooling til Strawberry shake) : 
dotnet add package StrawberryShake.Blazor --version 13.0.0-preview.65


list nuget pakker: 
 dotnet list .\NorwayMunicipalityPeaks.csproj package                                                                               
restore nuget pakker: 
dotnet restore

opprett tool manifest fil: (legges under .config)
dotnet new tool-manifest

legg til tool for StrawberryShake: 
dotnet tool install StrawberryShake.tools --prerelease       

generer en klient til en online GraphQl tjeneste, feks :
 dotnet graphql init https://api-crypto-workshop.chillicream.com/graphql -n CryptoClient   

 (dette er en service online som gir eksempeldata her - crypto currency sample data - kryptovaluta) 

 dotnet build

dotnet run watch

evt dotnet run 

trykk ctrl+shift+r to hot reload


