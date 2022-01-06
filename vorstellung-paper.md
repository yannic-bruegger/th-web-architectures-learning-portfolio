# Vorstellung: dapps im Web 4.0

dapps werden dezentralisierte Anwendungen genannt, die auf peer to peer und kryptographischen Verfahren aufbauen. In der letzten [Vorstellung zum Thema P2P](vorstellung-unused.md) wurde die Skalierbarkeit dieser Anwendungen hinterfragt. dapps in Kombination mit dem Web 4.0 sollen dieses Problem lösen. Es wird nicht mehr für jede Anwendung ein eigenes Netzwerk aufgebaut, sondern ein großes dezentrales Netz für mehrere Anwendungen. In der Praxis ist dieses Dezentrale Netzwerk eine Blockchain. Applikationen führen also Funktionalität auf der Blockchain aus, indem Transaktionen auf eben dieser durchgeführt werden. Da Blockchains üblicherweise Transaktionskosten verlangen, ist somit auch ein finanzieller Anreiz geschaffen. 

## Front-End
Der erste Vorteil für Entwickler ist, dass sich am Aufbau des Front-Ends kaum etwas ändert. Wie üblich können auf HTML, JavaScript und CSS gesetzt werden. Üblicherweise wird das Front-End klassisch über einen Server bereitgestellt. Die Interaktionen mit der Anwendungslogik (quasi das Backend) findet dann aber auf der Bockchain statt. Dafür muss sich der Benutzer erst Authentifizieren.

## Authentifizierung
Der erste große Unterschied zu herkömmlichen Applikationen ist die Authentisierung. Es ist nicht mehr nötig, sich gegenüber einem Authentifizierungsdienst (Google-Account; Microsoft-Account; Auth0; etc.) zu authentifizieren. Eine eindeutige Identifikation der NutzerInnen findet über die auf dem Rechner eingerichteten Wallets statt. Wallets sind ~Brieftaschen also eine Art Account um auf eine Blockchain zuzugreifen. Ein Wallet besteht letztendlich nur aus einem Schlüsselpaar. Der öffentliche Schlüssel (public key) kann verwendet werden, um Transaktionen zu empfangen. Der private Schlüssel (private key) kann verwendet werden um Transaktionen zu signieren (durchzuführen). Web-Applikationen können auf die APIs von Browser-Plugins zugreifen, die das Browser-Fenster mit einer ausgewählten Wallet verknüpfen. Ein Beispiel für so ein Plugin ist: [MetaMask](https://metamask.io/)

## Blockchain-Interaktionen
Ist der User mit einer Wallet authentifiziert, können Aktionen auf der Blockchain ausgeführt werden. Es gibt bereits zahlreiche Bibliotheken, die dafür eingesetzt werden können:
- ethers
- web3.js
- truffle
- embark

## Backend
Um an eine Transaktion auf der Blockchain eine Ablauflogik zu knüpfen, gibt es sogenannte Smart Contracts. Diese ersetzen das Backend und werden automatisch von der Blockchain durchgeführt, wenn bestimmte vorher definierte Bedingungen eintreffen. Eine Programmiersprache zum Schreiben von SMartContracts ist [Solidity](https://docs.soliditylang.org/en/v0.8.11/). Mithilfe eines Frameworks wie [Hardhat](https://hardhat.org/) lassen sich beispielsweise Smart Contracts auf der Etherium Blockchain entwickeln (erstellen, testen und veröffentlichen).

## Fazit
- P2P-Technologien wurden inzwischen in zusammenhang mit der Blockchain als solider theoretischer Ansatz für das Internet 4.0 anerkannt.
- Es kann jedoch sein, dass *die Blockchain* tatsächlich nur eine Tech-Bubble ist, die bald platzen wird.
- Es ist bereits so weit verbreitet, dass EntwicklerInnen (meiner Meinung nach) zumindest mal davon gehört haben sollten. Idealerweise auch mal ein kleines Hands-On-Projekt durchführen.
- Es bleiben viele Fragen offen. Wie funktionieren bisher "einfache" Komponenten einer Software im Web 4.0? Push Notifications zum Beispiel. Laufen die auch über die Blockchain? Gibt es dafür schon Libraries?

## Nützliche Links
- [Ethereum for Web Developers](https://link.springer.com/book/10.1007/978-1-4842-5278-9)
- [MetaMask Documentation](https://docs.metamask.io/guide/)
- [Get started with Solidity](https://karl.tech/learning-solidity-part-1-deploy-a-contract/)
- [Is Web3 all Hype? Top 10 Web 3.0 Questions & Answers](https://www.youtube.com/watch?v=wHTcrmhskto)

