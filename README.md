# StringArt
Making String Art image based on "String Art: Towards Computational Fabrication" article.

Example 1:
<p align="left">
  <img src="https://github.com/a-m-farahani/StringArt/blob/master/images/girl.jpg" height="200" title="Input Image">
  <img src="https://github.com/a-m-farahani/StringArt/blob/master/images/girl_result_circle.jpg" width="200" title="Result - Circle" >
  <img src="https://github.com/a-m-farahani/StringArt/blob/master/images/girl_result_square.jpg" width="200" title="Result - Square">
</p>

Example 2:
<p align="left">
  <img src="https://github.com/a-m-farahani/StringArt/blob/master/images/worldmap.jpg" height="200" title="Input Image">
  <img src="https://github.com/a-m-farahani/StringArt/blob/master/images/worldmap_result_circle.jpg" width="200" title="Result - Circle" >
  <img src="https://github.com/a-m-farahani/StringArt/blob/master/images/worldmap_result_square.jpg" width="200" title="Result - Square">
</p>

<b>Usage:</b>
<ul>
  <li> 
    <b>Circle:</b> <br/>
      converter = StringImageCircle(img_path, radius, nPins) <br/>
      result_img = converter.convert(max_lines=2500)
  </li>
  <li> 
    <b>Square:</b> <br/>
      converter = StringImageSquare(img_path, dim, nPins, noise=5) <br/>
      result_img = converter.convert(max_lines=2500)
  </li>
</ul>

Noise is used to reduce Moire effect on result image.
