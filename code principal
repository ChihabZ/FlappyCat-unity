using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class birdScript : MonoBehaviour
{


    public gamrlogicc logic;



    public Rigidbody2D MyRigidbody;
    public bool bichaLives = true;

    public float jumpForce;
    // Start is called before the first frame update
    void Start()
    {
        logic = GameObject.FindGameObjectWithTag("logic").GetComponent<gamrlogicc>();



    }


    void Update()
    {

        if (Input.GetKeyDown(KeyCode.Space) == true && bichaLives == true)
        {

            MyRigidbody.velocity = new Vector2(0, 1) * jumpForce;

        }
    }


    private void OnCollisionEnter2D(Collision2D collision)
    {
        logic.gameover();
        bichaLives = false;
    }
}
