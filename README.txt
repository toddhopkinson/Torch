README - iPhone LED Torch Singleton Component
Todd Hopkinson, 2010
===========================
Steps to use the LED Torch:

1. Drag Torch.h and Torch.m into your project

2. Place #import "Torch.h" in your implementation file in which you will access the Torch.

3. To access the torch, simply type:

     [[Torch sharedInstance] start];	// light me up!


4. Perhaps you want to have a button that toggles the torch on and off as follows:

-(IBAction)actionOnOffButton{

Torch *t = [Torch sharedInstance];

if([t isTorchOn])
{
		[t stop];
	}
	else
	{
		[t start];
	}

}

5. For some more fun, mess around with the 'startStrobesPerSecond' method.

Enjoy!

- Todd Hopkinson

