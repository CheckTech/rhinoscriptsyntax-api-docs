---
layout: bootstrap
---

# CurveCurveIntersection

Calculates intersection of two curve objects.
        

### Parameters:

- ***curveA*** = identifier of the first curve object.
- ***curveB*** = identifier of the second curve object. If omitted, then a
         self-intersection test will be performed on curveA.
tolerance [opt] = absolute tolerance in drawing units. If omitted,
                  the document's current absolute tolerance is used.
        

### Returns:


List of tuples of intersection information if successful.
The list will contain one or more of the following elements:
  Element Type     Description
  [n][0]  Number   The intersection event type, either Point (1) or Overlap (2).
  [n][1]  Point3d  If the event type is Point (1), then the intersection point 
                   on the first curve. If the event type is Overlap (2), then
                   intersection start point on the first curve.
  [n][2]  Point3d  If the event type is Point (1), then the intersection point
                   on the first curve. If the event type is Overlap (2), then
                   intersection end point on the first curve.
  [n][3]  Point3d  If the event type is Point (1), then the intersection point 
                   on the second curve. If the event type is Overlap (2), then
                   intersection start point on the second curve.
  [n][4]  Point3d  If the event type is Point (1), then the intersection point
                   on the second curve. If the event type is Overlap (2), then
                   intersection end point on the second curve.
  [n][5]  Number   If the event type is Point (1), then the first curve parameter.
                   If the event type is Overlap (2), then the start value of the
                   first curve parameter range.
  [n][6]  Number   If the event type is Point (1), then the first curve parameter.
                   If the event type is Overlap (2), then the end value of the
                   first curve parameter range.
  [n][7]  Number   If the event type is Point (1), then the second curve parameter.
                   If the event type is Overlap (2), then the start value of the
                   second curve parameter range.
  [n][8]  Number   If the event type is Point (1), then the second curve parameter.
                   If the event type is Overlap (2), then the end value of the 
                   second curve parameter range.
        
