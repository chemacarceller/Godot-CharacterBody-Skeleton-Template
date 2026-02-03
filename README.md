# Godot-CharacterBody-Skeleton-Template

This utility consists of a template for creating a character inheriting from...

Specifically, you want to obtain a CharacterBody3D object, and its mesh will be stored in a Skeleton3D.

The template includes a CollisionShape3D with a capsule-type shape prepared for a 1.80m high skeletal mesh.

This utility also contains an AnimationPlayer node and an AnimationTree node.

The script associated with this utility allows you to assign a Skeleton3D and an Animationplayer, both stored in PackedScenes.

When importing a character from mixamo, it is relatively easy to extract both the Skeleton3D and the Animationplayer and assign them to the character created from this template. 

This utility also has an additional Vector3 parameter to scale the Skeleton3D so that its height matches the 1.80 m height for which the CollisionShape3D is designed.

If you need a character of a different size than 1.80m or need a different collision mesh than the capsule, you can delete the default shape in your character and assign a custom one.

Finally, the template associates the Animationplayer assigned to the Animationtree node, but does not provide any root element of that node, in your character you will be responsible for assigning a value to that parameter

Feel free to extend the functionality of this template by adding components such as motion components, camera controller components, or adding multiple CollisionShape3Ds to make complex collision meshes (Note that only those meshes that hang directly from the character root node will be part of the global character collision mesh, collision meshes of nodes attached to the character root node will be ignored).

=====================================================================================

Esta utilidad consiste en una plantilla para crear un personaje heredado de...

En concreto, se desea obtener un objeto CharacterBody3D, cuya malla se almacenará en un Skeleton3D.

La plantilla incluye un CollisionShape3D con una forma tipo cápsula, preparado para una malla esquelética de 1,80 m de altura.

Esta utilidad también contiene los nodos AnimationPlayer y AnimationTree.

El script asociado a esta utilidad permite asignar un Skeleton3D y un Animationplayer, ambos almacenados en PackedScenes.

Al importar un personaje desde Mixamo, es relativamente fácil extraer tanto el Skeleton3D como el Animationplayer y asignarlos al personaje creado a partir de esta plantilla.

Esta utilidad también incluye un parámetro Vector3 adicional para escalar el Skeleton3D de modo que su altura coincida con la altura de 1,80 m para la que está diseñado el CollisionShape3D.

Si necesitas un personaje de un tamaño diferente a 1,80 m o una malla de colisión distinta a la de la cápsula, puedes eliminar la forma predeterminada de tu personaje y asignar una personalizada.

Finalmente, la plantilla asocia el Animationplayer asignado al nodo Animationtree, pero no proporciona ningún elemento raíz de ese nodo. En tu personaje, serás responsable de asignar un valor a ese parámetro.

Puedes ampliar la funcionalidad de esta plantilla añadiendo componentes como componentes de movimiento, componentes del controlador de cámara o múltiples CollisionShape3D para crear mallas de colisión complejas. (Ten en cuenta que solo las mallas que cuelgan directamente del nodo raíz del personaje formarán parte de la malla de colisión global del personaje; las mallas de colisión de los nodos asociados a dicho nodo se ignorarán).
