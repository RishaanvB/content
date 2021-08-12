---
title: XRSession.onselectstart
slug: Web/API/XRSession/onselectstart
tags:
- API
- AR
- Augmented Reality
- Event Handler
- Experimental
- Reference
- VR
- Virtual Reality
- WebXR
- WebXR Device API
- XRSession
- onselectstart
browser-compat: api.XRSession.onselectstart
---
<div>{{APIRef("WebXR Device API")}}</div>

<p><span class="seoSummary">The <code><strong>onselectstart</strong></code> attribute of
    the {{DOMxRef("XRSession")}} object is the event handler for the
    {{DOMxRef("XRSession.selectstart_event", "selectstart")}} event, which is dispatched
    when user starts making some sort of selection by pressing a trigger, touchpad, or
    button, speaking a command, or making a hand gesture. For example, this might include
    pressing a button or moving a joystick.</span></p>

<div class="notecard note">
  <p><strong>Note:</strong> Not to be confused with {{DOMxRef("XRSession.onselect")}}
    and {{DOMxRef("XRSession.onselectend")}}.</p>
</div>

<h2 id="Syntax">Syntax</h2>

<pre class="brush: js"><em>XRSession</em>.onselectstart = function(event) { ... }
</pre>

<h2 id="Example">Example</h2>

<pre class="brush: js"><em>XRSession</em>.onselectstart = function(event) {
  console.log("The user has started a primary action, but might not have completed it.")
}
</pre>

<h2 id="Specifications">Specifications</h2>

{{Specifications}}

<h2 id="Browser_compatibility">Browser compatibility</h2>

<p>{{Compat}}</p>

<h2 id="See_also">See also</h2>

<ul>
  <li>{{DOMxRef("XRSession.onselectend")}}</li>
  <li>{{DOMxRef("XRSession.onselect")}}</li>
</ul>