# Swift-UI-Reusable-View
The first step would be in XCode menu go to create a new file and select file type `SwiftUI View`.<br>
## File > New > File 
![Screenshot 2024-03-14 at 4 46 50 AM](https://github.com/danielurra/Swift-UI-Reusable-View/assets/51704179/09918fa5-4cf5-4b88-849b-017a9a617b43)<br>
## iOS > SwiftUI View
![Screenshot 2024-03-14 at 4 49 29 AM](https://github.com/danielurra/Swift-UI-Reusable-View/assets/51704179/054f66a2-c067-4495-bf88-d9620404947c)
## Name it CustomButtonView
See the boilerplate code below:<br>
![Screenshot 2024-03-14 at 5 00 05 AM](https://github.com/danielurra/Swift-UI-Reusable-View/assets/51704179/53efc93e-970f-4ac8-b4bb-ed53b601b082)
## Write the code for your view
![Screenshot 2024-03-14 at 4 54 49 AM](https://github.com/danielurra/Swift-UI-Reusable-View/assets/51704179/b7e55839-8e3d-49b2-b4c9-31e04f0ff175)
## Grab the code
```swift

import SwiftUI

struct CustomButtonView: View {
    
    var titleDanny: String
    var colorDanny: Color
    
    var body: some View {
        Text(titleDanny)
            .font(.body)
            .bold()
            .padding()
            .background(colorDanny)
            .foregroundStyle(.white)
            .clipShape(RoundedRectangle(cornerRadius: 15))
    }
}

#Preview {
    CustomButtonView(titleDanny: "Tap Me", colorDanny: .blue)
}

```
## Add action to a button
I know 2(two) ways to add a button, the easy one would be using the **Plus** symbol, see below:<br>
![Screenshot 2024-03-14 at 4 38 31 AM](https://github.com/danielurra/Swift-UI-Reusable-View/assets/51704179/5b98e829-7f05-4ffd-b403-a05e0c9c9c62)<br>
You simply select then drag and drop:<br>
![Screenshot 2024-03-14 at 4 39 00 AM](https://github.com/danielurra/Swift-UI-Reusable-View/assets/51704179/32f4095b-1e42-4dc4-8f42-1f8003d392a1)<br>
The second way is to manually type the following code:<br>
```swift
Button(action: {}){
                    CustomButtonView(titleDanny: "ALL CAPS", colorDanny: .red)
                }
```
![Screenshot 2024-03-14 at 4 32 34 AM](https://github.com/danielurra/Swift-UI-Reusable-View/assets/51704179/3b164119-b7f8-40a3-b5f8-b57e2fb46a0a)

