---
title: "Post: Code Fence Example"
excerpt_separator: "<!--more-->"
categories:
  - Blog
tags:
  - Post Formats
  - Programming
  - SwiftUI
---

## This is an example of a code fence with Swift syntax highlighting
### I will add a line in VS Code

`````swift
import SwiftUI

struct ContentView: View {
    @ObservedObject var dogVM = DogViewModel()
    @State private var backgroundIsGreen = false
    @State private var isLoading = false
    
    var body: some View {
        ZStack {
            Color(backgroundIsGreen ? .green : .white)
            VStack(spacing: 20) {
                Group {
                    if dogVM.image != nil {
                        Image(uiImage: dogVM.image!)
                            .resizable()
                            .frame(width: 320, height: 240)
                            .aspectRatio(contentMode: .fill)
                    } else {
                        Rectangle().stroke(lineWidth: 2).foregroundColor(.red)
                            .frame(width: 320, height: 240)
                    }
                }
                Button("Get Dog Image") {
                    Task {
                        await dogVM.getDog()
                    }
                }
                Button("Change Background") {
                    self.backgroundIsGreen.toggle()
                }
            }
        }
    }
}

#Preview {
    ContentView()
}

`````

