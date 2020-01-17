# node-red-contrib-binpacking

node-red-contrib-binpacking is based on the binpackingjs (https://github.com/olragon/binpackingjs) library.
it only supports 3D pakcing and is primarly designed for logistics purpose.

## Input / Output

### There is 2 inputs :

- A vehicle list called "bins". You must provide a msg.payload.bins as a json array.
- A parcel or package list you want to transport. You must provide a msg.payload.packages a a json array

### There is 1 output :

- The list of vehicle type with a success true or false ( { "success" : true}). true means the package can fit in the vehicle and false it means it can not. The result is available in the msg.payload.binpacking and the vehicle list order is kept. For each vehicle type the palette also provide which package can fit if they can all be in the vehicle.

## Test

You can check the flow in the sample directory to have a better understanding of the input and output.
It provides 2 examples :
- timestamp with predefined set of data
- api get/post to input values


## Contributors and Thanks

Thank you
@olragon for the binpackingjs library
@fanshan for the feedback on the palette
@misterbh for the first version
@zainiro for using it

LaV.
