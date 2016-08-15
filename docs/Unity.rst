============
Unity
============

This is the documentation for the Unity part.::

  using UnityEngine;

  public class GetComponentsInChildrenExample : MonoBehaviour
  {
    public Component[] hingeJoints;


    void Start( )
    {
        hingeJoints = GetComponentsInChildren<HingeJoint>( );

        foreach( HingeJoint joint in hingeJoints )
            joint.useSpring = false;
    }
  }
  
