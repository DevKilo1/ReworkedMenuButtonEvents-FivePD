Installation:
 - Drag and drop the .net.dll file into your fivepd/plugins folder!

**How it works:**
The following is the event format:
`FIVEPD::OnMenuTrigger:{MENU_TITLE}:{ITEM_TEXT}`
*Item text is in plain text, meaning without color or formatting codes.*

**Example Usage:**
```
EventHandlers["FIVEPD::OnMenuTrigger:Dispatch menu:Check license"] += new Action(() =>
            {
                Debug.WriteLine("Got check license button pressed!");
            });

```
**Refresh event:**
`FIVEPD::RefreshMenuTriggers`

**Example Usage:**

`BaseScript.TriggerEvent("FIVEPD::RefreshMenuTriggers");`

**This plugin automatically works with any FivePD addon menus. Running the refresh event is recommended after creating your new menu (if you care, of course)**