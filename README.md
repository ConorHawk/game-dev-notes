# Handy unity info

### Update() and FixedUpdate()

`Update()` runs every frame, as fast as your computer can process. It does not run at a consistent rate.

`FixedUpdate()` runs once per physics loop, which you can set in the project settings. It can be called more of less than `Update()`, and not necessarily in sync with it. It is used for physics when calculations need to be simulated at a certain rate to ensure consistency. When using physics based movement, it is best practice to use forces inside a `FixedUpdate()` functions.

### Physics based movement

`Time.delta` time returns the time it took to complete the last frame. Use this to avoid tying your calculations to the computers frame rate.
 
```C#
void FixedUpdate () {
	rb.AddForce(0,0,forwardForce * Time.deltaTime);
}
```

```C#
FindObjectOfType<GameManager>().EndGame();
```