
  <img src="https://komarev.com/ghpvc/?username=rakarmp&label=Profile%20Views&color=0e75b6&style=flat" alt="Profile visitor" />

```go
package main

import "fmt"

type Developer struct {
    Name   string
    Tools  []string
    OS     string
    GitHub string
}

func (dev Developer) Introduction() {
    fmt.Printf("Hi there!👋 I'm %s, a fresh graduate🎓 who's just plunged into the exciting world of web development💻.\n", dev.Name)
    fmt.Println("A huge fan of open source, I learn, build, and occasionally stumble in the realm of code.")
    fmt.Println("Let's learn and grow together.")
}

func (dev Developer) DisplayTools() {
    fmt.Println("Tools and languages I use:")
    for _, tool := range dev.Tools {
        fmt.Println("-", tool)
    }
}

func (dev Developer) DisplayOS() {
    fmt.Println("Operating System:", dev.OS)
}

func (dev Developer) DisplayGitHub() {
    fmt.Println("Find me on GitHub:", dev.GitHub)
}

func main() {
    tools := []string{
                      "Express", "JavaScript", "TypeScript", "Bash", "React",
                      "Node.js", "Next.js", "MongoDB", "HTML", "CSS", "Tailwind CSS",
                      "Bootstrap", "Markdown", "VSCode", "Git", "Golang",
                     }

    dev := Developer{
        Name:   "Raka Abdi Reza Maulana Putra ("良香"),
        Tools:  tools,
        OS:     "Linux (Arch)",
        GitHub: "https://github.com/rakarmp",
    }

    dev.Introduction()
    fmt.Println()
    dev.DisplayTools()
    fmt.Println()
    dev.DisplayOS()
    fmt.Println()
    dev.DisplayGitHub()
}

```
