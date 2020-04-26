# processing
// void setup 사이즈를 500,500으로 지정합니다. rectMode 행동하는 지점을 센터(중앙)으로 둡니다.
void setup(){ 
  size(500,500);
  rectMode(CENTER);
}
float f; // 변수를 실수로 지정하여 소숫점 값까지 기입할 수 있습니다.
void draw(){ 
  translate(mouseX,mouseY); // 이동시키는 translate함수에 mouseX,mouseY를 이용하여 마우스 커서위치에서 변화합니다.
  rotate(f);       // rotate f만큼 변환합니다.
  scale( sin(f)+0.1 ); // scale은 sin(f)+0.1만큼 바꿉니다.
  f = f+0.01;
  fill(0,0,0); // 색상
 rect(0,0,80,80); 
 fill(255,255,255);  //색상
 ellipse(0,0,80,80); // 원
}
