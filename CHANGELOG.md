**v1.4.5** Vec2D and Vec3D now support `copy` constructor where the original can be a duck-type. Further the only requirement is that the duck-type responds to `:x`, and `:y` by returning a `float` or `fixnum` thus Vec2D can be promoted to Vec3D (where `z = 0`), or more usually some other Vector or Point class can be used as the original. A `vector_utils` library has been implemented, see examples for usage.

**v1.4.4** Bump up to JRubyComplete-9.1.15.0

**v1.4.3** Features example sketches using the PixelFlow library by Thomas Diewald

**v1.4.2** Fix for windows `library_loader` thanks to Thomas Diewald

**v1.0.3** Initial version
