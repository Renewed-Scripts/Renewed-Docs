---
description: >-
  Here is all the exports for the script that you can incorporate into your own
  scripts
---

# 🚙 Exports

<pre class="language-lua"><code class="lang-lua">-- Client
exports['Renewed-Vehiclekeys']:hasKey(plate) -- Returns true/false if player has keys
exports['Renewed-Vehiclekeys']:addKey(plate) -- Adds a key to the specified player
exports['Renewed-Vehiclekeys']:removeKey(plate) -- Removes the key from a player
<strong>
</strong><strong>-- Server
</strong><strong>
</strong><strong>-- Removes the key from a player
</strong>exports['Renewed-Vehiclekeys']:removeKey(source, plate)

-- returns true/false if the player has the key
exports['Renewed-Vehiclekeys']:hasKey(source, plate)

-- Adds a key to the specified player
exports['Renewed-Vehiclekeys']:addKey(source, plate)
</code></pre>
