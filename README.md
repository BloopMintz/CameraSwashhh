# CameraSwashhh

using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class CamSwitch : MonoBehaviour {

  public GameObject cam1;   
	public GameObject cam2;   
	public GameObject cam3;   
	public GameObject cam4;
	public GameObject cam5;   
   
   //classes define the cameras
   
   //the if statements decide that when you press a key, it enables that specific camera and cancels out other cameras
   //so if the key 1 is pressed, camera 1 will be enabled while the others will be disabled
   void Update() {
        if (Input.GetButtonDown("1Key"))
       {
	cam1.SetActive(true);
	cam2.SetActive(false);
	cam3.SetActive(false);
	cam4.SetActive(false);
	cam5.SetActive(false);
       }
       if (Input.GetButtonDown("2Key"))
       {
	cam1.SetActive(false);
	cam2.SetActive(true);
	cam3.SetActive(false);
	cam4.SetActive(false);
	cam5.SetActive(false);
       }
       if (Input.GetButtonDown("3Key"))
       {
	cam1.SetActive(false);
	cam2.SetActive(false);
	cam3.SetActive(true);
	cam4.SetActive(false);
	cam5.SetActive(false);
       }
if (Input.GetButtonDown("4Key"))
       {
	cam1.SetActive(false);
	cam2.SetActive(false);
	cam3.SetActive(false);
	cam4.SetActive(true);
	cam5.SetActive(false);
       }
if (Input.GetButtonDown("5Key"))
       {
	cam1.SetActive(false);
	cam2.SetActive(false);
	cam3.SetActive(false);
	cam4.SetActive(false);
	cam5.SetActive(true);
       }
    }
}

