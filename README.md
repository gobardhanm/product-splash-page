# Product splash page

    > Responsive challenges..
    > Transform text
    > Viewport units
    > Style form elements
    > Flexbox order
    > Modifier classes
    > Box-sizing... Etc.

# CSS:

    > Text-shadow:

        Ex: 0 1px 2px #9cdh3d (horizontal shadow, vertical shadow , blur-radius for blur effect, hex-value)

    > Transforming text:

        Ex:
            text-transform: capitalize;

                - "capitalize" : first letter of each word is capitalize
                - "lowercase" : transform all text to lowercase
                - "uppercase" : transform all text to uppercase
    
    > Viewports units:
        Area within the browser window that displaying our site.

        - There are two units:

            - vh (viewport height)
                - 1vh is equal to 1% of the viewport height.
                *- min-height can help in stretching while scrooling.

            - vw (viewport width)
                - 1vw is equal to 1% of the viewport width.
                
    > We can use "background" for background color & background image.

        Ex: background-color: #3l35jd;
            background-image: url("images/pic.jpg")

            Can be written as:
                background: #3l35jd url("images/pic.jpg");

    > In "focus" state, we can often remove the default outline the browser gives it as long as we style the focus element differently.

    > In "form" the font don't usually inherit the font family set, so we have to set the font-family to inherit menually.

        Ex: font-family: inherit;

    > "letter-spacing" is useful to make sapce between letters.

        Ex: letter-spacing: 1px;

    > Reordering flex items:

        - With the "order" property, we can easily change the visual order of the flex items without thouching the "HTML".

        - Our flex items have a default order value of "0".

        Ex: 
             .tube {
                order: 0;
            }
             
             *// its default.

             .tube {
                order: -1;
            }

            *// shifts the flex item to the first.

            .tube {
                order: 1;
            }

            *// shifts the flex item to the end .

        Ex.2:

            .coat {
                order: 1;
            }

            .dish {
                order: 2;
            }

            .tube {
                order: 3;
            }

            .goggles {
                order: 4;
            }

        // we can order multiple items also, like this.

    > "box-sizing" :

        - The box-sizing property alter the way an element total width and height get calculated and the value "border-box" forces any padding and border into the elements total size instead of expanding it.

            Ex;
                border-sizing: border-box;


        *- "box-sizing" can be applied to any elements which accepts height and width.

        *> We can use "universal (*) selector" to select all the elements at once and apply the box-sizing.

            Ex: * {
                    box-sizing: border-box;    
                }

            *> For the pseudo elements, we should use:

                Ex:

                    *, *::before, *::after {
                        box-sizing: border-box;    
                    }