# StringArt
Making String Art images based on <a href="https://doi.org/10.1111/cgf.13359">String Art: Towards Computational Fabrication</a> article with a single connected thread or an Eulerian path in graph of N vertices.

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
* <b>Circle:</b> <br/> 
```python
converter = StringImageCircle(img_path, radius, nPins)
result_img = converter.Convert(max_lines=2500)
```

* <b>Square:</b>
```python
converter = StringImageSquare(img_path, dim, nPins, noise=5)
result_img = converter.Convert(max_lines=2500)
```

Adding Noise to Pin Positions is used to reduce <a href='https://en.wikipedia.org/wiki/Moir%C3%A9_pattern'>Moire effect</a> in result image.

A video example of string art conversion process (you need libx265 codec to play it): <a href='https://github.com/a-m-farahani/StringArt/blob/master/in_process.mp4'>Link</a>
<br/>
To see the lines data(starting pin and ending pin of each line) use converter.Lines: <br/>
print(converter.Lines)
