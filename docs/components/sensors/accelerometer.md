# Accelerometer
<p>Non-visible component that can detect shaking and measure acceleration approximately in three dimensions using SI units (m/s<sup>2</sup>).  The components are: </p>
<ul>
<li> <strong>xAccel</strong>: 0 when the phone is at rest on a flat      surface, positive when the phone is tilted to the right (i.e.,      its left side is raised), and negative when the phone is tilted      to the left (i.e., its right size is raised).</li>
 <li> <strong>yAccel</strong>: 0 when the phone is at rest on a flat      surface, positive when its bottom is raised, and negative when      its top is raised. </li>
 <li> <strong>zAccel</strong>: Equal to -9.8 (earth's gravity in meters per      second per second when the device is at rest parallel to the ground      with the display facing up,      0 when perpendicular to the ground, and +9.8 when facing down.       The value can also be affected by accelerating it with or against      gravity. </li></ul>
 <p></P>
 <h3>Properties</h3>
 <dl>
  <dt><code><em>Available</em></code></dt>
  <dd></dd>
  <dt><code>Enabled</code></dt>
  <dd></dd>
  <dt><code>LegacyMode</code> (designer only)</dt>
  <dd>Prior to the release that added this property the AccelerometerSensor
    component passed through sensor values directly as received from the
    Android system. However these values do not compensate for tablets
    that default to Landscape mode, requiring the MIT App Inventor
    programmer to compensate. However compensating would result in
    incorrect results in Portrait mode devices such as phones.
    We now detect Landscape mode tablets and perform the compensation.
    However if your project is already compensating for the change, you
    will now get incorrect results. Although our preferred solution is for
    you to update your project, you can also just set this property to “true”
    and our compensation code will be deactivated. Note: We recommend that
    you update your project as we may remove this property in a future
    release.</dd>
  <dt><code>MinimumInterval</code></dt>
  <dd>The minimum interval, in milliseconds, between phone shakes</dd>
  <dt><code>Sensitivity</code></dt>
  <dd>A number that encodes how sensitive the accelerometer is. The choices are: 1 = weak, 2 = moderate,  3 = strong.</dd>
  <dt><code><em>XAccel</em></code></dt>
  <dd></dd>
  <dt><code><em>YAccel</em></code></dt>
  <dd></dd>
  <dt><code><em>ZAccel</em></code></dt>
  <dd></dd>
</dl>
<h3>Events</h3>
<dl>
  <dt><code>AccelerationChanged(number xAccel, number yAccel, number zAccel)</code></dt>
  <dd>Indicates the acceleration changed in the X, Y, and/or Z dimensions.</dd>
  <dt><code>Shaking()</code></dt>
  <dd>Indicates the device started being shaken or continues to be shaken.</dd>
</dl>
<h3>Methods</h3>
"
none
"
