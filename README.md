Building Binary Counter
alt text
There are 4 numbers of LEDs, blinking of LED in combination with each other defines the Decimal numbers from 0 to 1.

In this code only till 6 Decimal LED binary program is done. Rest program are same, just have to make high and low looking at the conversion donts in the above image.

//declear variable or name pins/saying using those pins
int pin2 = 2;
int pin3 = 3;
int pin4 = 4;
int pin5 = 5;

void setup() 
{
    pinMode(pin2, OUTPUT);
    pinMode(pin3, OUTPUT);
    pinMode(pin4, OUTPUT);
    pinMode(pin5, OUTPUT);    
}

void loop()
{
    //Indicating zero
    digitalWrite(pin2, LOW);
    digitalWrite(pin3, LOW);
    digitalWrite(pin4, LOW);
    digitalWrite(pin5, LOW);
    delay(750);

    // Indicating One
    digitalWrite(pin2, LOW);
    digitalWrite(pin3, LOW);
    digitalWrite(pin4, LOW);
    digitalWrite(pin5, HIGH);
    delay(750);

    // Indicating Two
    digitalWrite(pin2, LOW);
    digitalWrite(pin3, LOW);
    digitalWrite(pin4, HIGH);
    digitalWrite(pin5, LOW);
    delay(750);

    // Indicating Three
    digitalWrite(pin2, LOW);
    digitalWrite(pin3, LOW);
    digitalWrite(pin4, HIGH);
    digitalWrite(pin5, HIGH);
    delay(750);

 // Indicating Four
    digitalWrite(pin2, LOW);
    digitalWrite(pin3, HIGH);
    digitalWrite(pin4, LOW);
    digitalWrite(pin5, LOW);
    delay(750);

    // Indicating Five
    digitalWrite(pin2, LOW);
    digitalWrite(pin3, HIGH);
    digitalWrite(pin4, LOW);
    digitalWrite(pin5, HIGH);
    delay(750);

     // Indicating Six
    digitalWrite(pin2, LOW);
    digitalWrite(pin3, HIGH);
    digitalWrite(pin4, HIGH);
    digitalWrite(pin5, HIGH);
    delay(750);
}
Circuit Diagram
alt text

Click Here for WOKWI Simulation circuit.

Click Here Paul McWhorter Arduino Tutorial 6, Build an LED Binary Counter

Arduino Analog Write Command
The analog pin of Arduon correspond to value between 0 and 255. 0V corresponds to 0 and 5V corresponds to 255. Its 2^8 meansing 8 bits: 1, 2, 4, 8, 16, 32, 64, 128, 256.

Change the value of brightness to 0 it will be turned off or change value 255< to make it dimmer.

int redPin = 9;
int brightness = 255;

void setup() 
{
    pinMode(redPin, OUTPUT);
}

void loop()
{
    analogWrite(redPin, brightness);
}
Circuit Diagram
alt text

Click Here for WOKWI Simulation circuit.

Click Here Paul McWhorter Arduino Tutorial 7, Analog Write Command
