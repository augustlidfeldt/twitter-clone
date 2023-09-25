## Twitter Clone

Initial setup:
Create T3 app
Start planetscale account and free-tier database (both dev and main branches)
Update the schema.prisma with the correct database information from planetscale
Start Discord Application (dev and prod) for authentication later
Populate all the env variables with information from both Discord and the Planetscale database
Setup git remote by creating GitHub repo
Go into Vercel, setup new project and select the correct Github repo
Add all env variables to Vercel and deploy
Now a deployed application should be up and running on Vercel accessible through a URL

### Creating a custom Button

If you want to create a custom object, like a button, that inherits all the properities of the normal Button you declare the type as follows:

import types {ButtonHTMLAttributes} from "react"; //import only the types from the components, found by hovering the normal button

// below type declares all the props

type ButtonProps = {
small?: boolean, //question mark means optional
gray?: boolean
} & DeatiledHTMLProps<ButtonHTMLAttributes>; // add the & sign between our special type and the original types

### Using the images from Next Auth

To access the images from next auth the next.config.mjs file needs to be updated, by adding the link to

### Using refs to style HTML component

To style the textarea component we use the useCallback() hook to grab the reference to the textArea as soon as the element is rendered. Inside the callback we also set a textAreaRef which has been initialized with the hook UseRef().

Setting a ref to the textarea makes it so that we can then use the textAreaRef on each render with the hook useLayoutEffect(). Inside of the function we call our custom function to set the textarea height and pass the reference to our textarea.

## Backend

### Setting up the TRPCRouter
