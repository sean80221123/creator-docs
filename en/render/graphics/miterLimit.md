# MiterLimit

The `MiterLimit` property sets or returns the maximum miter length.
The miter length refers to the distance between the inner and outer corners of the intersection of the two lines.

**Tip**: `miterLimit` is valid only if the `lineJoin` property is "miter".

The smaller the angle of the corners, the greater the length of the miter.
To avoid miter length getting too long, we can use the `miterLimit` property.
If the miter length exceeds the value of miterLimit, the corners are displayed with the "bevel" type of lineJoin

| Parameter | Description |
| -------------- | ----------- |
| number | positive number. Specifies the maximum miter length. If the miter length exceeds the value of miterLimit, the corners are displayed with the "bevel" type of lineJoin |

## Example

```javascript
var ctx = node.getComponent(cc.Graphics);
ctx.miterLimit = 10;
ctx.moveTo(20,20);
ctx.lineTo(100,50);
ctx.lineTo(20,100);
ctx.fill();
```

<a href="graphics/miterLimit.png"><img src="graphics/miterLimit.png"></a>

<hr>

Return to [Graphics Component Reference](../../components/graphics.md).
