# Nmap Setup on Windows

Je documente ici l'installation de mes outils de sécurité sur Windows. Pour commencer, voici comment j'ai installé et configuré Nmap.

## Ma config
- Windows 10/11 (64-bit)
- PowerShell
- Gestionnaire de paquets : `winget`

## Ce qu'il me fallait
- Windows 11
- PowerShell en mode Administrateur
- `winget` (normalement déjà installé sur les versions récentes de Windows)

## Installation

### 1. Vérifier si Nmap est déjà là
Avant de télécharger quoi que ce soit, j'ai vérifié si l'outil n'était pas déjà présent sur la machine.

```powershell
nmap --version
Test-Path "C:\Program Files (x86)\Nmap\nmap.exe"
Test-Path "C:\Program Files\Nmap\nmap.exe"
where.exe nmap
winget list --name nmap
