# Curve remove doubles addon for Blender 3D

# Curve remove doubles merged with Simplify Curves+ and now part of blender since 2.80 

Adds comand "Remove Dobles" for curves in Blender 3D
<p>Sometimes in exported curves in Blender, you can note bugs: some of the curve may not be traced, or artifacts on the extruded wall:</p>

<p><img alt="Снимок"height="375"width="429"class="lazy" src="http://multlabs.com/sites/default/files/2016-04/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202017-04-27%2016-17-39.png"></p>

<p>This is becouse of nearby points of Bezier curve. Of course, you can manually delete these points, restore the guides, but there is a faster and more efficient way: add-on "Curve Remove Doubles".</p>

<p>The addon glues nearby points on a single Bézier curve. In fact it is an analogue of the usual Remove Doubles on a mesh, but it is for a curve. But unlike the mesh one, it does not connect the points from different parts of the curves, even if they are on the ends of the two curves. To glue such points, you must first connect them with F-button.</p>

<h4>Download</h4>

<p><a href="https://raw.githubusercontent.com/crantisz/blender-curve-remove-doubles-addon/master/curve_remove_doubles.py">Addon file</a>. Download <em>curve_remove_doubles.py </em> and install like usual addon.</p>

<h4>How to use</h4>

<h5>Fixing curves</h5>

<p>Let we have a curve with troubles:</p>

<p><img alt="Снимок"height="375"width="429"class="lazy"src="http://multlabs.com/sites/default/files/2016-04/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202017-04-27%2016-17-39.png"></p>

<p>Select all poins, than press W -> Remove Doubles:</p>

<p><img alt="Снимок"height="489"width="869"class="lazy"src="http://multlabs.com/sites/default/files/2016-04/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202017-04-27%2016-17-392.png"></p>

<p>Look at result:</p>

<p><img alt="Снимок"height="66"width="435"class="lazy"src="http://multlabs.com/sites/default/files/2016-04/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202017-04-27%2016-18-25_0.png"></p>

<a name='p5' id='p5' class='navigatorancor'></a><h5>Connecting two curves with preservation of guides</h5>

<p>Let we have some curves to connecting</p>

<p><img alt="Снимок"height="346"width="801"class="lazy"src="http://multlabs.com/sites/default/files/2016-04/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202017-04-27%2016-27-12.png"></p>

<p>First, make segment with F-button. Next W -> Remove Doubles:</p>

<p><img alt="Снимок"height="374"width="540"class="lazy"src="http://multlabs.com/sites/default/files/2016-04/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202017-04-27%2016-28-47.png"></p>

<p>If the points don't stuck together - probably they are further than the established limit, press F6 and increase the limit until they are stuck together:</p>

<p><img alt="Снимок"height="92"width="375"class="lazy"src="http://multlabs.com/sites/default/files/2016-04/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202017-04-27%2016-57-56.png"></p>

<p>Look at result:</p>

<p><img alt="Снимок"height="466"width="477"class="lazy"src="http://multlabs.com/sites/default/files/2016-04/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202017-04-27%2016-28-55.png"></p>

<p> </p>
