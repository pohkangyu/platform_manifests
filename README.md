"# platform_manifests" 

repo init -u https://github.com/pohkangyu/platform_manifests.git
<br>
repo sync -j4
<br>
#Command to remove the anbox dependancies
<br>
<br>
rm -rf system/core && rm -rf frameworks/base && rm -rf frameworks/native && rm -rf frameworks/av && rm -rf device/generic/goldfish && rm -rf device/generic/goldfish-opengl && rm -rf hardware/libhardware && rm -rf hardware/interfaces && rm -rf vendor/anbox
<br>
<br>
#Command to git revert
<br>
<br>
cd system/vold && git checkout e37a2acb459d9a0a1ce25c4c0abf33ba824ea978 && cd ~/Desktop/anbox10/ &&
cd system/core && git checkout 5aa0e4241029c80617a8e98b07f7f48ab6b3a3d7 && cd ~/Desktop/anbox10/ &&
cd frameworks/base && git checkout c0fbdf45d7c9826533186751a03c27e500cac78e && cd ~/Desktop/anbox10/ &&
cd frameworks/native && git checkout 2173449d9dccb15b87c9df5d373dc32e1dcabed6 && cd ~/Desktop/anbox10/ &&
cd frameworks/av && git checkout cee606de904204e96447ae9010ab40bb151bf3bf && cd ~/Desktop/anbox10/ &&
cd device/generic/goldfish && git checkout c1752fc13b9b42fa713f2c4bff39cd2b42ffbdd8 && cd ~/Desktop/anbox10/ &&
cd device/generic/goldfish-opengl && git checkout 7aed9b4344b307de827567d3f8498bfbd978fe34 && cd ~/Desktop/anbox10/ &&
cd hardware/libhardware &&  git checkout 8e03635abbb0428c13ae8727ecc7c54d40bb923f && cd ~/Desktop/anbox10/ &&
cd hardware/interfaces && git checkout 4dd458dab6c7a29fc5394fd20b1e7931a3caabec && cd ~/Desktop/anbox10/
