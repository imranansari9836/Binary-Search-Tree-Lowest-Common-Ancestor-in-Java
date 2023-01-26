public static Node lca(Node root, int v1, int v2) {
      if(Math.max(v1, v2) < root.data)
      {
       return lca(root.left, v1, v2);
      }
     else if(Math.min(v1, v2) > root.data){
          return lca(root.right, v1, v2); 
          }
      
          return root;

    }
