# Braceml

>  Brace markup language - generate html and css using comfy s expressions 

```lisp
(Template "a-container" [title href]
    (div 
        (class "template-div")
        (a (href $href) 
            (h3 $title)
        )
    )
)

(content
    (div
        (h1 "Language showcase")
        (For $e [["Github" "https://github.com/xnacly"]
            (Apply "a-container" (Get $e 0) (Get $e 1))
        )
    )
)

(meta
    (title "Language showcase")
)

(style
    ($main "#fff")
    (a.custom
        (color $main)
    )
)
```

## Usage

Braceml ships a compiler and a repl for fast iterating and quick testing. 

## In depth guide

### Document structure

### Element attributes

### Templates

### Control flow

#### Variables

#### Objects

#### Lists

#### Loops

