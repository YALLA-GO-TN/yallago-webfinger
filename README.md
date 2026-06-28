# yallago-webfinger

Dépôt technique — Infrastructure Yalla-Go

## Rôle

Ce dépôt héberge le fichier WebFinger de l'entreprise Yalla-Go.
Il permet à Tailscale de vérifier que l'identité des comptes 
@yalla-go.com est gérée par ZITADEL.

## Fonctionnement

Le fichier `.well-known/webfinger` est servi via GitHub Pages 
sur le domaine yalla-go.com.

Tailscale vérifie ce fichier lors de la connexion avec un 
fournisseur OIDC custom.

## Structure

.well-known/
    └── webfinger       # Fichier JSON — ne pas modifier sans validation

## Fournisseur d'identité

ZITADEL Cloud — auth.yalla-go.com

## ⚠️ Attention

Ne pas modifier le contenu du fichier webfinger sans valider 
l'impact sur Tailscale et ZITADEL.
Toute modification doit être validée par le coordinateur technique.

## Contact

ops@yalla-go.com
