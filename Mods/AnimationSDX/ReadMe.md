AnimationSDX
=======================

Provides a Mecanim animation layer for use for external entities to control their animations. This version does not support Root Motion, so that must be disabled in the animator component of the Unity3d bundle and in XML as shown below.

A sample entityclass entry called SDXTemplate is provided as an easy way to include the MecanimSDX class. It extends off of the zombieTemplateMale.

Example Usage:
--------------

~~~~~~~~~~~{.xml}
 <configs>
    <append xpath="/entity_classes">
      <entity_class name="SDXTemplate" extends="zombieTemplateMale">
        <property name="AvatarController" value="MecanimSDX, Mods" />
        <property name="RootMotion" value="false" />
      </entity_class>
    </append>
</configs>
~~~~~~~~~~~