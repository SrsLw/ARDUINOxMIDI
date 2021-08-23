void setup() {
  // Connectionspeed for MIDI
  Serial.begin(31250);

}

void loop() {
  // Send Note On Message(0x90) for Note 57(0x39) at Velocity 127(0x7F)
  sendMessage(0x90, 0x39, 0x7F);
  
  delay(1000);

  // Send Note off Message(0x90) for Note 57(0x39). Velocity does not matter
  sendMessage(0x80, 0x39, 0x00);

  delay(1000);
}

void sendMessage(byte byteOne, byte byteTwo, byte byteThree) {
  Serial.write(byteOne);
  Serial.write(byteTwo);
  Serial.write(byteThree);
}
