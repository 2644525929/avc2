# include < stdio .h >
# include < time .h >
extern "C" int init(int d_lev);
extern "C" int Sleep( int sec , int usec );
extern "C" int set_motor( int motor , int spieed );
extern "C" char get_pixel(int row,int col,int colour);
extern "C" take_picture();
int main (){
int v_right;
int v_left;
init (0);
int sum=0;
v_right = 100;
v_left = 100;
int i;
int w;
int s;
int ai[15];


take_picture();
for(i=0,i<16,i++){
w=get_pixel(i*20,120,3);
if(w>127){ai[i]=1;}
else{ai[i]=0;}
if(ai[i]==0&&ai[i+1]==1){
int st=i;
}
if(ai[i]==1&&ai[i+1]==0){
int end=i;
}
float center=(st+end)/2;
float err = center-7.5;
int v_right=15
printf("%d%n",w);
