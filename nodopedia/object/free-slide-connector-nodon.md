---
layout: entry
title:  "Free-Slide-Connector Nodon"
category: object
order: 23
quote: Check the Nodopedia? You mean like read the<br />instructions? Pfff, no way! I do my own thing!
---
<h1>Port</h1>
<h2>Input</h2>
<table class="wrapped">
  <colgroup>
    <col />
    <col />
    <col />
  </colgroup>
  <tbody>
    <tr>
      <th>Port name</th>
      <th>Port function</th>
      <th>Input operation</th>
    </tr>
    <tr>
      <td label="Port name"><span>X</span></td>
      <td label="Port function"><span>Sets how far away the object is placed along the x-axis relative to its original position, taking the input value from this port as the distance. Measured in meters.<br />Movement force will be applied to any objects connected to it, above or below.<br /><br />If nothing is connected to this port, an input value of 0.00 will be assumed.</span></td>
      <td label="Input operation"><span>Signal passes through unchanged</span></td>
    </tr>
    <tr>
      <td label="Port name"><span>Y</span></td>
      <td label="Port function"><span>Sets how far away the object is placed along the y-axis relative to its original position, taking the input value from this port as the distance. Measured in meters.<br />Movement force will be applied to any objects connected to it, above or below.<br /><br />If nothing is connected to this port, an input value of 0.00 will be assumed.</span></td>
      <td label="Input operation"><span>Signal passes through unchanged</span></td>
    </tr>
    <tr>
      <td label="Port name"><span>Z</span></td>
      <td label="Port function"><span>Sets how far away the object is placed along the z-axis relative to its original position, taking the input value from this port as the distance. Measured in meters.<br />Movement force will be applied to any objects connected to it, above or below.<br /><br />If nothing is connected to this port, an input value of 0.00 will be assumed.</span></td>
      <td label="Input operation"><span>Signal passes through unchanged</span></td>
    </tr>
  </tbody>
</table>
<h2>Output</h2>
<p>None</p>
<h2>Connection</h2>
<table class="wrapped">
  <colgroup>
    <col />
    <col />
  </colgroup>
  <thead>
    <tr>
      <th>
        <p>Port name</p>
      </th>
      <th>
        <p>Port function</p>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td label="Port name"><span>Upper connection port</span></td>
      <td label="Port function">
        <p>Connect this port to the lower connection port of another Nodon to physically link objects.<br>
        <br>You can have both the upper and lower connected objects move along all three axes.<br>
        <br>Object Nodon, Fancy-Object Nodon, Text-Object Nodon, Number-Object Nodon, Moving-Object Nodon, and Rotating-Object Nodon can connect to this connection port only with their lower connection ports.</p>
      </td>
    </tr>
    <tr>
      <td label="Port name"><span>Lower connection port</span></td>
      <td label="Port function">
        <p>This is a special type of port that physically links objects generated by Nodon on the game screen. Connect it to the upper connection port of another Nodon to link them.<br>
        <br>You can have both the upper and lower connected objects move along all three axes.<br>
        <br>Person Nodon, Car Nodon, UFO Nodon, Object Nodon, Fancy-Object Nodon, Text-Object Nodon, Number-Object Nodon, Moving-Object Nodon, and Rotating-Object Nodon can connect to this connection port only with the upper connection port.</p>
      </td>
    </tr>
  </tbody>
</table>
<h1>Settings</h1>
<h2>Slide Motion Input</h2>
<p>This property can be set individually for the X, Y, and Z ports.<br />When set on, the value of the input determines the amount of parallel movement.<br />When set off, the input will be ignored, and the object can be moved freely by an external force in parallel along that direction.<br />There's no limit to the movement distance.</p>
<h2>Position</h2>
<p>Determines the position of the object at the time of game start or after a reset.<br />X, Y, and Z can each be set to between -100.00 and 100.00.<br />Measured in meters.</p>