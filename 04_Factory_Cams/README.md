# Bitwise XOR on Images

Requires ImageMagick
Technique is discussed at: http://stackoverflow.com/questions/8504882/searching-for-a-way-to-do-bitwise-xor-on-images

convert ./camera_feed_overlap_error.png ./a-img_out-5.png -fx "(((255*u)&(255*(1-v)))|((255*(1-u))&(255*v)))/255" b-img_out-clw.png
cp b-img_out-clw.png c-img_out-clw.png
convert ./b-img_out-clw.png ./factory_cam_1.png -fx "(((255*u)&(255*(1-v)))|((255*(1-u))&(255*v)))/255" b-img_out-clw-1.png
convert ./b-img_out-clw-1.png ./factory_cam_2.png -fx "(((255*u)&(255*(1-v)))|((255*(1-u))&(255*v)))/255" b-img_out-clw-1-2.png
convert ./b-img_out-clw-1-2.png ./factory_cam_3.png -fx "(((255*u)&(255*(1-v)))|((255*(1-u))&(255*v)))/255" b-img_out-clw-1-2-3.png
convert ./b-img_out-clw-1-2-3.png ./factory_cam_4.png -fx "(((255*u)&(255*(1-v)))|((255*(1-u))&(255*v)))/255" b-img_out-clw-1-2-3-4.png
 
convert ./b-img_out-clw-1-2-3.png ./factory_cam_5.png -fx "(((255*u)&(255*(1-v)))|((255*(1-u))&(255*v)))/255" b-img_out-clw-1-2-3-5.png
 
convert ./b-img_out-clw-1-2.png ./factory_cam_4.png -fx "(((255*u)&(255*(1-v)))|((255*(1-u))&(255*v)))/255" b-img_out-clw-1-2-4.png
convert ./b-img_out-clw-1-2-4.png ./factory_cam_5.png -fx "(((255*u)&(255*(1-v)))|((255*(1-u))&(255*v)))/255" b-img_out-clw-1-2-4-5.png
 
convert ./b-img_out-clw-1.png ./factory_cam_3.png -fx "(((255*u)&(255*(1-v)))|((255*(1-u))&(255*v)))/255" b-img_out-clw-1-3.png
convert ./b-img_out-clw-1-3.png ./factory_cam_4.png -fx "(((255*u)&(255*(1-v)))|((255*(1-u))&(255*v)))/255" b-img_out-clw-1-3-4.png
convert ./b-img_out-clw-1-3-4.png ./factory_cam_5.png -fx "(((255*u)&(255*(1-v)))|((255*(1-u))&(255*v)))/255" b-img_out-clw-1-3-4-5.png
 
convert ./b-img_out-clw.png ./factory_cam_2.png -fx "(((255*u)&(255*(1-v)))|((255*(1-u))&(255*v)))/255" b-img_out-clw-2.png
convert ./b-img_out-clw-2.png ./factory_cam_3.png -fx "(((255*u)&(255*(1-v)))|((255*(1-u))&(255*v)))/255" b-img_out-clw-3.png
convert ./b-img_out-clw-3.png ./factory_cam_4.png -fx "(((255*u)&(255*(1-v)))|((255*(1-u))&(255*v)))/255" b-img_out-clw-2-3-4.png
convert ./b-img_out-clw-2-3-4.png ./factory_cam_5.png -fx "(((255*u)&(255*(1-v)))|((255*(1-u))&(255*v)))/255" b-img_out-clw-2-3-4-5.png

