# Static Site Generators

![s](https://user-images.githubusercontent.com/116082827/235368538-3b501a2b-e9e5-43c8-a69d-90a4fbb3155b.png)


Static site generators are tools that generate static HTML, CSS, and JavaScript files from templates and content. They can be used to create fast, secure, and scalable websites that are easy to deploy and maintain. Some popular static site generators include Jekyll, Hugo, and Gatsby. Here's an example of using Gatsby to create a simple blog:





import React from 'react';

import { graphql } from 'gatsby';



export default function BlogPost({ data }) {

  const post = data.markdownRemark;



  return (

    <div>

      <h1>{post.frontmatter.title}</h1>

      <div dangerouslySetInnerHTML={{ __html: post.html }} />

    </div>

  );

}



export const query = graphql`

  query($slug: String!) {

    markdownRemark(fields: { slug: { eq: $slug } }) {

      frontmatter {

        title

      }

      html

    }

  }

`;

In this code, we're using Gatsby to create a blog post template. 
