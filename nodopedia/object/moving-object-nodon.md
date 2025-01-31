---
layout: entry
title:  "Moving-Object Nodon"
category: object
order: 6
quote: Working up a sweat yet?<br />I put objects on the game screen, and I move 'em too!
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
      <td label="Port function">
        <p>Moves the object along the x-axis in response to the input received at this port.<br />A negative value will move in the X- direction, and a positive value will move in the X+ direction.</p>
      </td>
      <td label="Input operation"><span>Restricted to between -100.00 and 100.00</span></td>
    </tr>
    <tr>
      <td label="Port name"><span>Y</span></td>
      <td label="Port function">
        <p>Moves the object along the y-axis in response to the input received at this port.<br />A negative value will move in the Y- direction, and a positive value will move in the Y+ direction.</p>
      </td>
      <td label="Input operation"><span>Restricted to between -100.00 and 100.00</span></td>
    </tr>
    <tr>
      <td label="Port name"><span>Z</span></td>
      <td label="Port function">
        <p>Moves the object along the z-axis in response to the input received at this port.<br />A negative value will move in the Z- direction, and a positive value will move in the Z+ direction.</p>
      </td>
      <td label="Input operation"><span>Restricted to between -100.00 and 100.00</span></td>
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
  <tbody>
    <tr>
      <th>Port name</th>
      <th>Port function</th>
    </tr>
    <tr>
      <td label="Port name"><span>Upper connection port</span></td>
      <td label="Port function">
        <p>Connect this port to the lower connection port of another Nodon to physically link objects.<br><br>Connects to all lower connection ports.</p>
      </td>
    </tr>
    <tr>
      <td label="Port name"><span>Lower connection port</span></td>
      <td label="Port function">
        <p>This is a special type of port that physically links objects generated by Nodon on the game screen. Connect it to the upper connection port of another Nodon to link them.<br><br>When connected to this port, the object will be physically linked to the target object.<br><br>Person Nodon, Car Nodon, UFO Nodon, Object Nodon, Fancy-Object Nodon, Text-Object Nodon, Number-Object Nodon, Moving-Object Nodon, Rotating-Object Nodon, all connector Nodon, Head Nodon, and Hand Nodon can connect to this connection port only with their upper connection ports.</p>
      </td>
    </tr>
  </tbody>
</table>
<h1>Settings</h1>
<h2>Object Shape</h2>
<p>Sets the shape.<br />You can choose from Box, Cylinder, or Sphere.</p>
<h2>Properties</h2>
<p>Sets the properties of objects.</p>
<p>The following properties can be enabled or disabled: Visible, Solid, Destructive, Destructible, Play Sound When Hit/Destroyed?, or Can Be Grabbed by Hand Nodon?<br />Movable is always enabled.</p>
<p>See also: <a href="/nodopedia/tips/properties">About Properties</a></p>
<h2>Color</h2>
<p>Sets the color.</p>
<table class="wrapped">
  <colgroup>
    <col />
    <col />
  </colgroup>
  <thead>
    <tr>
      <th>
        <p>Setting value</p>
      </th>
      <th>
        <p>Description</p>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td label="Setting value"><span>Auto</span></td>
      <td label="Description">
        <p>The color will be applied automatically, depending on the properties.<br><br>See also: <a href="/nodopedia/tips/automatic-colors">When Color Is Set to Auto</a></p>
      </td>
    </tr>
    <tr>
      <td label="Setting value"><span>Blue<br />Red<br />Green<br />Yellow<br />Light blue<br />Pink<br />Lime green<br />Orange<br />Purple<br />Brown<br />White<br />Black</span></td>
      <td label="Description"><span>Changes the color as specified.</span></td>
    </tr>
  </tbody>
</table>
<h2>Material</h2>
<p>Sets the type of material.</p>
<table class="wrapped">
  <thead>
    <tr>
      <th>
        <p>Setting value</p>
      </th>
      <th>
        <p>Description</p>
      </th>
    </tr>
    <tr>
      <td label="Setting value"><span>Normal</span></td>
      <td label="Description"><span>The basic material for objects.</span></td>
    </tr>
    <tr>
      <td label="Setting value"><span>Bouncy</span></td>
      <td label="Description"><span>A rubberlike material. Bouncy and hard to slip on.</span></td>
    </tr>
    <tr>
      <td label="Setting value"><span>Slippery</span></td>
      <td label="Description"><span>An ice-like material with a slippery surface.</span></td>
    </tr>
    <tr>
      <td label="Setting value"><span>Floaty</span></td>
      <td label="Description"><span>A lighter-than-air, balloon-like material that floats upward.</span></td>
    </tr>
    <tr>
      <td label="Setting value"><span>Zero gravity</span></td>
      <td label="Description"><span>A strange material that neither falls nor floats upward!</span></td>
    </tr>
  </thead>
</table>
<h2>Connection Type</h2>
<p>Sets the firmness of the connection to the target object.</p>
<table class="wrapped">
  <colgroup>
    <col />
    <col />
  </colgroup>
  <thead>
    <tr>
      <th>
        <p>Setting value</p>
      </th>
      <th>
        <p>Description</p>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td label="Setting value"><span>Normal</span></td>
      <td label="Description"><span>Affixes firmly to the target object.</span></td>
    </tr>
    <tr>
      <td label="Setting value"><span>Springy</span></td>
      <td label="Description"><span>Sticks softly to the target object, as if linked by a spring.</span></td>
    </tr>
    <tr>
      <td label="Setting value"><span>180° Rotation</span></td>
      <td label="Description"><span>Moves freely around the target object, as if connected by a half-sphere.</span></td>
    </tr>
  </tbody>
</table>
<h2>Connection Point</h2>
<p>Sets how the objects physically connect to each other. A connection point is defined based on an object's face.</p>
<table class="wrapped">
  <colgroup>
    <col />
    <col />
  </colgroup>
  <thead>
    <tr>
      <th>
        <p>Setting value</p>
      </th>
      <th>
        <p>Description</p>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td label="Setting value"><span>Auto</span></td>
      <td label="Description"><span>Chooses the closest connection points of the objects automatically based on factors such as location, orientation, and size of the objects.</span></td>
    </tr>
    <tr>
      <td label="Setting value"><span>Manual</span></td>
      <td label="Description"><span>The objects will be joined by the faces set in the Own Connection Point and Target Connection Point options.</span></td>
    </tr>
  </tbody>
</table>
<h2>Own Connection Point</h2>
<p>The face indicated on this object will join to the face indicated in the Target Connection Point option.<br />You can choose from Center, X-, X+, Y-, Y+, Z-, or Z+.<br />Only effective when Connection Point is set to Manual.</p>
<h2>Target Connection Point</h2>
<p>The face indicated on the target object will join to the face indicated in the Own Connection Point option.<br />You can choose from Center, X-, X+, Y-, Y+, Z-, or Z+.<br />Only effective when Connection Point is set to Manual.</p>
<h2>Frame of Reference<br />for Motion</h2>
<p>Sets which rules an object will base its movement on.</p>
<table class="wrapped">
  <colgroup>
    <col />
    <col />
  </colgroup>
  <thead>
    <tr>
      <th>
        <p>Setting value</p>
      </th>
      <th>
        <p>Description</p>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td label="Setting value"><span>World</span></td>
      <td label="Description"><span>Moves the object along the world's coordinate system, according to the input received.<br />The world's coordinate system is based on the world's directionality, regardless of the directionality of the camera or the object itself.</span></td>
    </tr>
    <tr>
      <td label="Setting value"><span>Local</span></td>
      <td label="Description"><span>Moves the object along the local coordinate system, according to the input received.<br />The local coordinate system is based on the directionality of the object itself.</span></td>
    </tr>
    <tr>
      <td label="Setting value"><span>Camera</span></td>
      <td label="Description"><span>Moves the object along the camera's coordinate system, according to the input received.<br />The camera's coordinate system is based on the directionality of the camera's viewpoint.</span></td>
    </tr>
  </tbody>
</table>
<h2>Mode</h2>
<p>Sets how the object is moved in response to the input value.</p>
<table class="wrapped">
  <colgroup>
    <col />
    <col />
  </colgroup>
  <tbody>
    <tr>
      <th>Setting value</th>
      <th>Description</th>
    </tr>
    <tr>
      <td label="Setting value"><span>Acceleration</span></td>
      <td label="Description"><span>The value received at the X, Y, or Z port is treated as acceleration, with the input acceleration added to the object's current speed.<br />The input is measured in meters per second squared.</span></td>
    </tr>
    <tr>
      <td label="Setting value"><span>Speed</span></td>
      <td label="Description"><span>The value received at the X, Y, or Z port is treated as the target speed. The object's speed will be adjusted until it matches the input value.<br />The input is measured in meters per second.</span></td>
    </tr>
  </tbody>
</table>
<h2>Size</h2>
<p>Sets the size of an object.<br />When the object's shape is set to Box, you'll be able to set the X, Y, and Z<br />dimensions separately.<br />When the object's shape is set to Cylinder, the ratio between X and Z will be fixed, but their ratios to Y can be adjusted.<br />When the object's shape is set to Sphere, the ratio between X, Y, and Z will be fixed.<br /><br />X, Y, and Z can be set to between 0.10 and 10.00. Measured in meters.</p>
<h2>Position</h2>
<p>Determines the position of the object at the time of game start or after a reset.<br />X, Y, and Z can each be set to between -100.00 and 100.00.<br />Measured in meters.<br />However, if Movable is enabled and the world's shape is set to Plane, Dome, Cuboid, or Cylinder, the Y value will be adjusted so that objects lower than Y: 0 aren't embedded into the ground.</p>
<h2>Rotation</h2>
<p>Sets the orientation of the object at game start or after a reset.<br />The X, Y, and Z axes can each be set between -180.00° and 180.00°.</p>