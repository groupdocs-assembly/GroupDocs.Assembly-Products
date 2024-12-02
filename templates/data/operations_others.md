    items: 
          
        # operation loop 1
        - name: "<% "{common-content.operations.barcode.name}" %>"
          operation: "barcode"
          link: "/assembly/<% get "ProdCode" %>/barcode/<% get "FileFormat" %>/"
          description: "<% "{common-content.operations.barcode.description}" %>"

        # operation loop 2
        - name: "<% "{common-content.operations.diagram.name}" %>"
          operation: "diagram"
          link: "/assembly/<% get "ProdCode" %>/diagram/<% get "FileFormat" %>/"
          description: "<% "{common-content.operations.diagram.description}" %>"

        # operation loop 3
        - name: "<% "{common-content.operations.document.name}" %>"
          operation: "document"
          link: "/assembly/<% get "ProdCode" %>/document/<% get "FileFormat" %>/"
          description: "<% "{common-content.operations.document.description}" %>"

        # operation loop 4
        - name: "<% "{common-content.operations.list.name}" %>"
          operation: "list"
          link: "/assembly/<% get "ProdCode" %>/list/<% get "FileFormat" %>/"
          description: "<% "{common-content.operations.list.description}" %>"

        # operation loop 5
        - name: "<% "{common-content.operations.table.name}" %>"
          operation: "table"
          link: "/assembly/<% get "ProdCode" %>/table/<% get "FileFormat" %>/"
          description: "<% "{common-content.operations.table.description}" %>"
         
          