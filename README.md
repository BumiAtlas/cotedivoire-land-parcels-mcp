# Côte d'Ivoire Rural Land Parcels & Certificate Lookup MCP

[Français](#français)

Connect your AI assistant (Claude, ChatGPT, Cursor) to [BumiAtlas](https://bumiatlas.com) for Ivorian rural land research through the Model Context Protocol (MCP).

This listing is a focused entry point for:

- ~68k rural parcels with a land-certificate dossier from AFOR's (Agence Foncière Rurale) Géoportail du Foncier Rural: individual (CFI) and collective (CFC) certificates
- Parcel lookup by parcel code or dossier number (`283-011-000001`), village (narrowed by department), or coordinates
- Certification status (in progress or certified), filing, certification and rejection dates, the surveying project and operator, declared and surveyed area in hectares
- Satellite and street map images of a parcel and its neighbours, labelled by parcel code

This is the rural-certificate layer, not the legal cadastre. 

## Connect

```
https://bumiatlas.com/mcp/cotedivoire
```

Add it as a custom connector in any MCP client and sign in with Google. Tools, examples and data notes: [bumiatlas.com/mcp-docs/cotedivoire](https://bumiatlas.com/mcp-docs/cotedivoire).

- **Claude:** Settings → Connectors → Add custom connector, paste the URL, then Connect.
- **ChatGPT:** Settings → Apps & Connectors → Advanced → Developer mode, then Create with the URL and OAuth authentication.

## Tools

| Tool | Description |
|---|---|
| `CI_parcel_search` | Find parcels by parcel code or dossier number, village (paged), or `latitude, longitude`; each result is the whole record, the boundary as GeoJSON on request |
| `CI_parcel_image` | Satellite or street map image of a parcel or point, with every parcel in view outlined and labelled with its parcel code |

## Example prompts

- *"Which rural parcel is at 6.8276, -5.2893? Is it certified?"*
- *"Look up dossier 283-011-000001."*
- *"List the AFOR parcels in a village with their surveyed areas."*
- *"How does the declared area compare with the surveyed one?"*

## Data source

Parcels © Agence Foncière Rurale (AFOR), Côte d'Ivoire, Géoportail du Foncier Rural. A copy of public data for research, not a legal land record.

## Français

Connectez votre assistant IA (Claude, ChatGPT ou Cursor) à [BumiAtlas](https://bumiatlas.com) via le Model Context Protocol (MCP) pour vos recherches sur le foncier rural en Côte d'Ivoire.

- ~68 000 parcelles rurales avec un dossier de certificat foncier (CFI ou CFC) de l'AFOR
- Recherche par code parcelle, numéro de dossier, village ou coordonnées
- Statut de certification, dates, superficies déclarée et levée

Les noms des détenteurs et des demandeurs ne sont pas inclus.

**Connexion :** ajoutez `https://bumiatlas.com/mcp/cotedivoire` comme connecteur personnalisé dans votre client MCP et connectez-vous avec Google. Les noms des outils sont en anglais, mais l'assistant peut répondre en français.
