---
layout: entry
title:  "Camera Nodon"
category: object
order: 33
quote: If you're particular about your camera<br />angles, you've run into the right Nodon.
---
<h1>If you call up this Nodon...</h1>
<p>This Nodon will capture the game screen according to the Nodon's location, direction, and settings.</p>
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
      <td label="Port name"><span>Up/Down</span></td>
      <td label="Port function">
        <p>Moves the camera's direction up or down depending on the value received as input.<br />Positive values will move it up, and negative values will move it down.</p>
      </td>
      <td label="Input operation"><span>Restricted to between -1.00 and 1.00</span></td>
    </tr>
    <tr>
      <td label="Port name"><span>Horizontal</span></td>
      <td label="Port function"><span>Moves the camera's direction horizontally depending on the value received as input.<br />Positive values will move it right, and negative values will move it left.</span></td>
      <td label="Input operation"><span>Restricted to between -1.00 and 1.00</span></td>
    </tr>
    <tr>
      <td label="Port name"><span>Reset</span></td>
      <td label="Port function"><span>If an input with a value other than 0.00 is received, the camera's position and orientation will reset.</span></td>
      <td label="Input operation"><span>Determines whether a signal is or is not equal to 0.00</span></td>
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
      <td label="Port name"><span>Lower connection port</span></td>
      <td label="Port function">
        <p>This is a special type of port that physically links objects generated by Nodon on the game screen. Connect it to the upper connection port of another Nodon to link them.<br>
        <br>When physically connected to an object, the camera will track the connected object.<br>
        <br>Person Nodon, Car Nodon, UFO Nodon, Object Nodon, Fancy-Object Nodon, Text-Object Nodon, Number-Object Nodon, Moving-Object Nodon, and Rotating-Object Nodon can only connect to this connection port with their upper connection ports.<br />You can't connect to a connection group that includes a Head Nodon or a Hand Nodon.</p>
      </td>
    </tr>
  </tbody>
</table>
<h1>Settings</h1>
<h2>Horizontal Tracking Rate</h2>
<p>Sets how closely the horizontal movement of the connected object, or the position represented by input received, will be tracked. If it's set to 0.00, it won't follow at all. If it's set to 1.00, it'll move immediately to the target.<br />Can be set to between 0.00 and 1.00.</p>
<h2>Vertical Tracking Rate</h2>
<p>Sets how closely the vertical movement of the connected object, or the position represented by input received, will be tracked. If it's set to 0.00, it won't follow at all. If it's set to 1.00, it'll move immediately to the target.<br />Can be set to between 0.00 and 1.00.</p>
<h2>Camera Field of View</h2>
<p>Sets the horizontal angle of the area framed by the camera.<br />Can be between 10.00 and 120.00. Measured in degrees (°).</p>
<h2>Track Character's Y Rotation</h2>
<p>Sets whether or not the camera will track the object when it rotates.<br />Only effective when connected to the Person Nodon, Car Nodon, or UFO Nodon.</p>
<h2>Position</h2>
<p>Determines the position of the object at the time of game start or after a reset.<br />X, Y, and Z can each be set to between -100.00 and 100.00.<br />Measured in meters.</p>
<p>Effective only when not connected to an object.</p>
<h2>Offset Distance</h2>
<p>Sets the distance that the camera is offset by.<br />You can set it from between -100.00 to 100.00. Measured in meters.</p>
<h2>X-Axis Rotation</h2>
<p>Sets the orientation of the object at game start or after a reset, according to x-axis rotation.</p>
<p>Can be set between -90.00° and 90.00°.</p>
<h2>Y-Axis Rotation</h2>
<p>Sets the orientation of the object at game start or after a reset, according to y-axis rotation.</p>
<p>Can be set between -180.00° and 180.00°.</p>
<h1>Other</h1>
<p>Moves as shown below, depending on the connection status and offset distance.</p>
<table class="wrapped">
  <colgroup>
    <col />
    <col />
    <col />
  </colgroup>
  <tbody>
    <tr>
      <th>
        <br />
      </th>
      <th>No connection</th>
      <th>Connection</th>
    </tr>
    <tr>
      <th class="hide_mobile">Distance of 0.00</th>
      <td label="Distance of 0.00 / No connection"><span>The Camera Nodon's position will be used as the camera's position and will capture the game screen in the direction indicated by the amount of rotation set in the Camera Nodon. Vertical and horizontal movement rotates the camera's point of focus in relation to its position.</span></td>
      <td label="Distance of 0.00 / Connection"><span>The connected object's position will be used as the camera's position and will capture the game screen in the direction indicated by the amount of rotation set in the Camera Nodon. Vertical and horizontal movement rotates the camera's point of focus in relation to its position.</span></td>
    </tr>
    <tr>
      <th class="hide_mobile">Distance other than 0.00</th>
      <td label="Distance other than 0.00 / No connection"><span>The Camera Nodon's position will be used as the camera's target and will capture the game screen from a position determined by the value set in the Offset Distance. Vertical and horizontal movement rotates the camera's position around the target.</span></td>
      <td label="Distance other than 0.00 / Connection"><span>The connected object's position will be used as the camera's target and will capture the game screen from a position determined by the value set in the Offset Distance. Vertical and horizontal movement rotates the camera's position around the target.</span></td>
    </tr>
  </tbody>
</table>
<p>You can only call one Camera Nodon per game.<br />Also, you can't call other camera-related Nodon at the same time as a Camera Nodon.</p>