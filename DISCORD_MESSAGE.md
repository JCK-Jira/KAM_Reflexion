# Message Discord avec @everyone (notification tous les membres)

```
@everyone
🏛 **KAM INC. — Ma réflexion du jour · 17/04/2026** · 07H16 CET

🟢 GC #1 · HAUSSIER FAIBLE
🟢 ES #2 · HAUSSIER
🟢 NQ #3 · HAUSSIER FORT
🟢 RTY #4 · HAUSSIER
🔻 WTI #5 · BAISSIER FAIBLE

🔗 https://jck-jira.github.io/KAM_Reflexion/17-04-2026.html
```

## Version JSON webhook (avec mention @everyone et embed OG)

```json
{
  "content": "@everyone\n🏛 **KAM INC. — Ma réflexion du jour · 17/04/2026** · 07H16 CET",
  "allowed_mentions": { "parse": ["everyone"] },
  "embeds": [
    {
      "title": "KAM INC. — Ma réflexion du jour · 17/04/2026",
      "description": "**07H16 CET**\n\n🟢 **GC #1** · HAUSSIER FAIBLE\n🟢 **ES #2** · HAUSSIER\n🟢 **NQ #3** · HAUSSIER FORT\n🟢 **RTY #4** · HAUSSIER\n🔻 **WTI #5** · BAISSIER FAIBLE\n\n[🔗 Consulter l'analyse complète](https://jck-jira.github.io/KAM_Reflexion/17-04-2026.html)",
      "color": 16751104,
      "image": { "url": "https://jck-jira.github.io/KAM_Reflexion/og-17042026.png?v=17042026" },
      "footer": { "text": "KAM INC. · 17/04/2026 · Confidentiel · 50% TP1 / 50% TP2 · BE dès TP1" }
    }
  ]
}
```

## ⚠️ Permissions @everyone

Le rôle du webhook doit avoir la permission **"Mentionner @everyone, @here et tous les rôles"** dans les paramètres du canal Discord. Sinon la mention s'affichera mais ne déclenchera pas la notification push.

Vérification : `Paramètres du canal > Permissions > Webhook > Mentionner @everyone = activé`
