- A scene: consider this as the stage where every object needs to be added in order to be rendered
- A camera: in this case we will use a perspective camera, but it could also be an orthographic camera.
- A renderer that will display all the scene using WebGL.
- One or more objects to render, in our case, we will create a plane, a sea and a sky (a few clouds)
- One or more lights: there is also different types of lights available. In this project we will mainly use a hemisphere light for the atmosphere and a directional light for the shadows.



1. create a scene:

2. create an object:

	create a geometry : 
		BoxGeometry, BufferGeometry, CircleGeometry, ConeGeometry, CubeGeometry, CylinderGeometry, DodecahedronGeometry, EdgesGeometry, 	ExtrudeGeometry, IcosahedronGeometry, InstancedBufferGeometry, LatheGeometry, OctahedronGeometry, ParametricGeometry, PlaneGeometry, PolyhedronGeometry, RingGeometry, ShapeGeometry, SphereGeometry, TetrahedronGeometry, TextGeometry, TorusGeometry, TorusKnotGeometry, TubeGeometry, WireframeGeometry
		
		BufferGeometry:
		This class is an efficient alternative to Geometry, because it stores all data, including vertex positions, face indices, normals, colors, UVs, and custom attributes within buffers; this reduces the cost of passing all this data to the GPU.
		This also makes BufferGeometry harder to work with than Geometry; rather than accessing position data as Vector3 objects, color data as Color objects, and so on, you have to access the raw data from the appropriate attribute buffer. This makes BufferGeometry best-suited for static objects where you don't need to manipulate the geometry much after instantiating it.
		
	create a material
	pass them into a mesh
	add the mesh to our scene

3. Add object to scene