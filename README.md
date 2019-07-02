# hello-world
NO.1 of JTY repository

#include<opencv2/opencv.hpp>
#include<iostream>
 
using namespace cv;
using namespace std;

int main(int argc, char** argv)
{
  Mat src;
  src = imread("1.jpg");
  if(!src.data)
  {
    printf("could not find image");
    return -1;
  }
  namedWindow("input",CV_WINDOW_AUTOSIZE);
  imshow("input",src);
  
  waitKey(0);
  return(0);
}
