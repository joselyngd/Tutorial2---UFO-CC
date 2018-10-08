\\https://github.com/joselyngd/Tutorial2---UFO-CC

using UnityEngine;
using System.Collections;

public class CameraController : MonoBehaviour
{

    public GameObject player;      


    private Vector3 offset;      

    void Start()
    {
        offset = transform.position - player.transform.position;
    }

    void LateUpdate()
    {
        transform.position = player.transform.position + offset;
    }
}
