---
title: XRSessionEvent.session
slug: Web/API/XRSessionEvent/session
tags:
- API
- AR
- Mixed
- Property
- Reality
- Reference
- Session
- VR
- Virtual
- WebXR
- WebXR API
- WebXR Device API
- XR
- XRSession
- XRSessionEvent
- augmented
- events
- sessions
browser-compat: api.XRSessionEvent.session
---
<p>{{APIRef("WebXR Device API")}}</p>

<p>The read-only {{domxref("XRSessionEvent")}} interface's
    <code><strong>session</strong></code> property indicates which
    {{domxref("XRSession")}} the event is about.</p>

<h2 id="Syntax">Syntax</h2>

<pre class="brush: js"><em>xrSession</em> = xrSessionEvent.<em>session</em>;
</pre>

<h3 id="Value">Value</h3>

<p>An {{domxref("XRSession")}} object indicating which WebXR session the event refers to.
</p>

<h2 id="Examples">Examples</h2>

<p>In this example, the <code>session</code> property is used to obtain the session object
  to manage when an event is received.</p>

<pre class="brush: js">xrSession.addEventListener("visibilitychange", e =&gt; {
  switch(e.session.visibilityState) {
    case "hidden":
      myEnableRendering(true);
      break;
    case "visible":
    case "visible-blurred":
      myEnableRendering(false);
      break;
  }
});
</pre>

<p>This calls a function that reacts to the session's visibility state change.</p>

<h2 id="Specifications">Specifications</h2>

{{Specifications}}

<h2 id="Browser_compatibility">Browser compatibility</h2>

<div>{{Compat}}</div>