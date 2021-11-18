// Pin 2 has an pushbutton connected on most Arduino boards.
// give it a name:
int pushButton = 2;
int led = 13;
bool go = false;

// the setup routine runs once when you press reset:
void setup() {
  //initialize serial communication at 9600 buts per second
  Serial.begin(9600);
  //make the pushButton's pin an input:
  pinMode(pushButton,INPUT);
  pinMode(led, OUTPUT);
}

// the loop routine runs over and over again forever:
void loop() {
  
  //read the input pin
  int buttonState = digitalRead(pushButton);
  Serial.println(buttonState);
  delay(1);
  //read the output pin
  if(buttonState > 0 ) {
  go = !go;
    delay(100);
  
  } 
  
  if(go == true)
  {
  digitalWrite(led, HIGH);
  }
  else
  {
     digitalWrite(led, LOW);
  }
}
