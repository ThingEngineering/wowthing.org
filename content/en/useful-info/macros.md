---
title: Macros
description: >
    Random useful macros
weight: 1
---

## Teleport to graveyard

```text
/script C_PartyInfo.InviteUnit("aaaaaaaaaaaaaa"); C_Timer.After(1, function() C_PartyInfo.LeaveParty(1) end)
```
