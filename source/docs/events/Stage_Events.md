title: HTML5 Canvas Special Stage Events Konva
---

All events are starts from Shapes. So if you click on an empty space on the canvas `click` then the event will not be triggered on any `Layer` and the event will not even be triggered on the `Stage` object. But if you really need to listen for `click` (or any other similar event) on a `Konva.Stage` on empty space you can:
1. Create a transparent rectange of the same size as the Stage and add it at the bottom of your shapes.
2. Or listen for special "content" events.

Supported content events:
contentMouseover, contentMousemove, contentMouseout, contentMousedown, contentMouseup, contentClick, contentDblclick, contentTouchstart, contentTouchmove, contentTouchend, contentTap, contentDblTap

Instruction: click everywhere. see console.

{% iframe /downloads/code/events/Stage_Events.html %}

{% include_code Konva Stage Events Demo events/Stage_Events.html %}
