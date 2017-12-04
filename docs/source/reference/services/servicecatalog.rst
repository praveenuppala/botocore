

**************
ServiceCatalog
**************

.. contents:: Table of Contents
   :depth: 2


======
Client
======



.. py:class:: ServiceCatalog.Client

  A low-level client representing AWS Service Catalog::

    
    client = session.create_client('servicecatalog')

  
  These are the available methods:
  
  *   :py:meth:`~ServiceCatalog.Client.accept_portfolio_share`

  
  *   :py:meth:`~ServiceCatalog.Client.associate_principal_with_portfolio`

  
  *   :py:meth:`~ServiceCatalog.Client.associate_product_with_portfolio`

  
  *   :py:meth:`~ServiceCatalog.Client.associate_tag_option_with_resource`

  
  *   :py:meth:`~ServiceCatalog.Client.can_paginate`

  
  *   :py:meth:`~ServiceCatalog.Client.copy_product`

  
  *   :py:meth:`~ServiceCatalog.Client.create_constraint`

  
  *   :py:meth:`~ServiceCatalog.Client.create_portfolio`

  
  *   :py:meth:`~ServiceCatalog.Client.create_portfolio_share`

  
  *   :py:meth:`~ServiceCatalog.Client.create_product`

  
  *   :py:meth:`~ServiceCatalog.Client.create_provisioning_artifact`

  
  *   :py:meth:`~ServiceCatalog.Client.create_tag_option`

  
  *   :py:meth:`~ServiceCatalog.Client.delete_constraint`

  
  *   :py:meth:`~ServiceCatalog.Client.delete_portfolio`

  
  *   :py:meth:`~ServiceCatalog.Client.delete_portfolio_share`

  
  *   :py:meth:`~ServiceCatalog.Client.delete_product`

  
  *   :py:meth:`~ServiceCatalog.Client.delete_provisioning_artifact`

  
  *   :py:meth:`~ServiceCatalog.Client.describe_constraint`

  
  *   :py:meth:`~ServiceCatalog.Client.describe_copy_product_status`

  
  *   :py:meth:`~ServiceCatalog.Client.describe_portfolio`

  
  *   :py:meth:`~ServiceCatalog.Client.describe_product`

  
  *   :py:meth:`~ServiceCatalog.Client.describe_product_as_admin`

  
  *   :py:meth:`~ServiceCatalog.Client.describe_product_view`

  
  *   :py:meth:`~ServiceCatalog.Client.describe_provisioned_product`

  
  *   :py:meth:`~ServiceCatalog.Client.describe_provisioning_artifact`

  
  *   :py:meth:`~ServiceCatalog.Client.describe_provisioning_parameters`

  
  *   :py:meth:`~ServiceCatalog.Client.describe_record`

  
  *   :py:meth:`~ServiceCatalog.Client.describe_tag_option`

  
  *   :py:meth:`~ServiceCatalog.Client.disassociate_principal_from_portfolio`

  
  *   :py:meth:`~ServiceCatalog.Client.disassociate_product_from_portfolio`

  
  *   :py:meth:`~ServiceCatalog.Client.disassociate_tag_option_from_resource`

  
  *   :py:meth:`~ServiceCatalog.Client.generate_presigned_url`

  
  *   :py:meth:`~ServiceCatalog.Client.get_paginator`

  
  *   :py:meth:`~ServiceCatalog.Client.get_waiter`

  
  *   :py:meth:`~ServiceCatalog.Client.list_accepted_portfolio_shares`

  
  *   :py:meth:`~ServiceCatalog.Client.list_constraints_for_portfolio`

  
  *   :py:meth:`~ServiceCatalog.Client.list_launch_paths`

  
  *   :py:meth:`~ServiceCatalog.Client.list_portfolio_access`

  
  *   :py:meth:`~ServiceCatalog.Client.list_portfolios`

  
  *   :py:meth:`~ServiceCatalog.Client.list_portfolios_for_product`

  
  *   :py:meth:`~ServiceCatalog.Client.list_principals_for_portfolio`

  
  *   :py:meth:`~ServiceCatalog.Client.list_provisioning_artifacts`

  
  *   :py:meth:`~ServiceCatalog.Client.list_record_history`

  
  *   :py:meth:`~ServiceCatalog.Client.list_resources_for_tag_option`

  
  *   :py:meth:`~ServiceCatalog.Client.list_tag_options`

  
  *   :py:meth:`~ServiceCatalog.Client.provision_product`

  
  *   :py:meth:`~ServiceCatalog.Client.reject_portfolio_share`

  
  *   :py:meth:`~ServiceCatalog.Client.scan_provisioned_products`

  
  *   :py:meth:`~ServiceCatalog.Client.search_products`

  
  *   :py:meth:`~ServiceCatalog.Client.search_products_as_admin`

  
  *   :py:meth:`~ServiceCatalog.Client.terminate_provisioned_product`

  
  *   :py:meth:`~ServiceCatalog.Client.update_constraint`

  
  *   :py:meth:`~ServiceCatalog.Client.update_portfolio`

  
  *   :py:meth:`~ServiceCatalog.Client.update_product`

  
  *   :py:meth:`~ServiceCatalog.Client.update_provisioned_product`

  
  *   :py:meth:`~ServiceCatalog.Client.update_provisioning_artifact`

  
  *   :py:meth:`~ServiceCatalog.Client.update_tag_option`

  

  .. py:method:: accept_portfolio_share(**kwargs)

    

    Accepts an offer to share a portfolio.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/AcceptPortfolioShare>`_    


    **Request Syntax** 
    ::

      response = client.accept_portfolio_share(
          AcceptLanguage='string',
          PortfolioId='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type PortfolioId: string
    :param PortfolioId: **[REQUIRED]** 

      The portfolio identifier.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {}
        
      **Response Structure** 

      

      - *(dict) --* 
    

  .. py:method:: associate_principal_with_portfolio(**kwargs)

    

    Associates the specified principal ARN with the specified portfolio.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/AssociatePrincipalWithPortfolio>`_    


    **Request Syntax** 
    ::

      response = client.associate_principal_with_portfolio(
          AcceptLanguage='string',
          PortfolioId='string',
          PrincipalARN='string',
          PrincipalType='IAM'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type PortfolioId: string
    :param PortfolioId: **[REQUIRED]** 

      The portfolio identifier.

      

    
    :type PrincipalARN: string
    :param PrincipalARN: **[REQUIRED]** 

      The ARN representing the principal (IAM user, role, or group).

      

    
    :type PrincipalType: string
    :param PrincipalType: **[REQUIRED]** 

      The principal type. Must be ``IAM``  

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {}
        
      **Response Structure** 

      

      - *(dict) --* 
    

  .. py:method:: associate_product_with_portfolio(**kwargs)

    

    Associates a product with a portfolio.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/AssociateProductWithPortfolio>`_    


    **Request Syntax** 
    ::

      response = client.associate_product_with_portfolio(
          AcceptLanguage='string',
          ProductId='string',
          PortfolioId='string',
          SourcePortfolioId='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type ProductId: string
    :param ProductId: **[REQUIRED]** 

      The product identifier.

      

    
    :type PortfolioId: string
    :param PortfolioId: **[REQUIRED]** 

      The portfolio identifier.

      

    
    :type SourcePortfolioId: string
    :param SourcePortfolioId: 

      The identifier of the source portfolio to use with this association.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {}
        
      **Response Structure** 

      

      - *(dict) --* 
    

  .. py:method:: associate_tag_option_with_resource(**kwargs)

    

    Associate a TagOption identifier with a resource identifier.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/AssociateTagOptionWithResource>`_    


    **Request Syntax** 
    ::

      response = client.associate_tag_option_with_resource(
          ResourceId='string',
          TagOptionId='string'
      )
    :type ResourceId: string
    :param ResourceId: **[REQUIRED]** 

      The resource identifier.

      

    
    :type TagOptionId: string
    :param TagOptionId: **[REQUIRED]** 

      The TagOption identifier.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {}
        
      **Response Structure** 

      

      - *(dict) --* 
    

  .. py:method:: can_paginate(operation_name)

        
    Check if an operation can be paginated.
    
    :type operation_name: string
    :param operation_name: The operation name.  This is the same name
        as the method name on the client.  For example, if the
        method name is ``create_foo``, and you'd normally invoke the
        operation as ``client.create_foo(**kwargs)``, if the
        ``create_foo`` operation can be paginated, you can use the
        call ``client.get_paginator("create_foo")``.
    
    :return: ``True`` if the operation can be paginated,
        ``False`` otherwise.


  .. py:method:: copy_product(**kwargs)

    

    Copies the specified source product to the specified target product or a new product.

     

    You can copy the product to the same account or another account. You can copy the product to the same region or another region.

     

    This operation is performed asynchronously. To track the progress of the operation, use  DescribeCopyProductStatus .

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/CopyProduct>`_    


    **Request Syntax** 
    ::

      response = client.copy_product(
          AcceptLanguage='string',
          SourceProductArn='string',
          TargetProductId='string',
          TargetProductName='string',
          SourceProvisioningArtifactIdentifiers=[
              {
                  'string': 'string'
              },
          ],
          CopyOptions=[
              'CopyTags',
          ],
          IdempotencyToken='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type SourceProductArn: string
    :param SourceProductArn: **[REQUIRED]** 

      The Amazon Resource Name (ARN) of the source product.

      

    
    :type TargetProductId: string
    :param TargetProductId: 

      The ID of the target product. By default, a new product is created.

      

    
    :type TargetProductName: string
    :param TargetProductName: 

      A name for the target product. The default is the name of the source product.

      

    
    :type SourceProvisioningArtifactIdentifiers: list
    :param SourceProvisioningArtifactIdentifiers: 

      The IDs of the product versions to copy. By default, all provisioning artifacts are copied.

      

    
      - *(dict) --* 

      
        - *(string) --* 

        
          - *(string) --* 

          
    
  
  
    :type CopyOptions: list
    :param CopyOptions: 

      The copy options. If the value is ``CopyTags`` , the tags from the source product are copied to the target product.

      

    
      - *(string) --* 

      
  
    :type IdempotencyToken: string
    :param IdempotencyToken: **[REQUIRED]** 

      A token to disambiguate duplicate requests. You can use the same input in multiple requests, provided that you also specify a different idempotency token for each request. 

      This field is autopopulated if not provided.

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'CopyProductToken': 'string'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **CopyProductToken** *(string) --* 

          A unique token to pass to ``DescribeCopyProductStatus`` to track the progress of the operation.

          
    

  .. py:method:: create_constraint(**kwargs)

    

    Creates a new constraint. For more information, see `Using Constraints <http://docs.aws.amazon.com/servicecatalog/latest/adminguide/constraints.html>`__ .

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/CreateConstraint>`_    


    **Request Syntax** 
    ::

      response = client.create_constraint(
          AcceptLanguage='string',
          PortfolioId='string',
          ProductId='string',
          Parameters='string',
          Type='string',
          Description='string',
          IdempotencyToken='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type PortfolioId: string
    :param PortfolioId: **[REQUIRED]** 

      The portfolio identifier.

      

    
    :type ProductId: string
    :param ProductId: **[REQUIRED]** 

      The product identifier.

      

    
    :type Parameters: string
    :param Parameters: **[REQUIRED]** 

      The constraint parameters. Expected values vary depending on which **Type** is specified. For more information, see the Examples section.

       

      For Type ``LAUNCH`` , the ``RoleArn`` property is required. 

       

      For Type ``NOTIFICATION`` , the ``NotificationArns`` property is required.

       

      For Type ``TEMPLATE`` , the ``Rules`` property is required.

      

    
    :type Type: string
    :param Type: **[REQUIRED]** 

      The type of the constraint. Case-sensitive valid values are: ``LAUNCH`` , ``NOTIFICATION`` , or ``TEMPLATE`` . 

      

    
    :type Description: string
    :param Description: 

      The text description of the constraint.

      

    
    :type IdempotencyToken: string
    :param IdempotencyToken: **[REQUIRED]** 

      A token to disambiguate duplicate requests. You can use the same input in multiple requests, provided that you also specify a different idempotency token for each request.

      This field is autopopulated if not provided.

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ConstraintDetail': {
                'ConstraintId': 'string',
                'Type': 'string',
                'Description': 'string',
                'Owner': 'string'
            },
            'ConstraintParameters': 'string',
            'Status': 'AVAILABLE'|'CREATING'|'FAILED'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ConstraintDetail** *(dict) --* 

          The resulting detailed constraint information.

          
          

          - **ConstraintId** *(string) --* 

            The identifier of the constraint.

            
          

          - **Type** *(string) --* 

            The type of the constraint.

            
          

          - **Description** *(string) --* 

            The text description of the constraint.

            
          

          - **Owner** *(string) --* 

            The owner of the constraint.

            
      
        

        - **ConstraintParameters** *(string) --* 

          The resulting constraint parameters.

          
        

        - **Status** *(string) --* 

          The status of the current request.

          
    

  .. py:method:: create_portfolio(**kwargs)

    

    Creates a new portfolio.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/CreatePortfolio>`_    


    **Request Syntax** 
    ::

      response = client.create_portfolio(
          AcceptLanguage='string',
          DisplayName='string',
          Description='string',
          ProviderName='string',
          Tags=[
              {
                  'Key': 'string',
                  'Value': 'string'
              },
          ],
          IdempotencyToken='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type DisplayName: string
    :param DisplayName: **[REQUIRED]** 

      The name to use for display purposes.

      

    
    :type Description: string
    :param Description: 

      The text description of the portfolio.

      

    
    :type ProviderName: string
    :param ProviderName: **[REQUIRED]** 

      The name of the portfolio provider.

      

    
    :type Tags: list
    :param Tags: 

      Tags to associate with the new portfolio.

      

    
      - *(dict) --* 

        Key-value pairs to associate with this provisioning. These tags are entirely discretionary and are propagated to the resources created in the provisioning.

        

      
        - **Key** *(string) --* **[REQUIRED]** 

          The ``ProvisioningArtifactParameter.TagKey`` parameter from  DescribeProvisioningParameters .

          

        
        - **Value** *(string) --* **[REQUIRED]** 

          The desired value for this key.

          

        
      
  
    :type IdempotencyToken: string
    :param IdempotencyToken: **[REQUIRED]** 

      A token to disambiguate duplicate requests. You can use the same input in multiple requests, provided that you also specify a different idempotency token for each request.

      This field is autopopulated if not provided.

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'PortfolioDetail': {
                'Id': 'string',
                'ARN': 'string',
                'DisplayName': 'string',
                'Description': 'string',
                'CreatedTime': datetime(2015, 1, 1),
                'ProviderName': 'string'
            },
            'Tags': [
                {
                    'Key': 'string',
                    'Value': 'string'
                },
            ]
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **PortfolioDetail** *(dict) --* 

          The resulting detailed portfolio information.

          
          

          - **Id** *(string) --* 

            The identifier for the portfolio.

            
          

          - **ARN** *(string) --* 

            The ARN assigned to the portfolio.

            
          

          - **DisplayName** *(string) --* 

            The name to use for display purposes.

            
          

          - **Description** *(string) --* 

            The text description of the portfolio.

            
          

          - **CreatedTime** *(datetime) --* 

            The UTC timestamp of the creation time.

            
          

          - **ProviderName** *(string) --* 

            The name of the portfolio provider.

            
      
        

        - **Tags** *(list) --* 

          Tags successfully associated with the new portfolio.

          
          

          - *(dict) --* 

            Key-value pairs to associate with this provisioning. These tags are entirely discretionary and are propagated to the resources created in the provisioning.

            
            

            - **Key** *(string) --* 

              The ``ProvisioningArtifactParameter.TagKey`` parameter from  DescribeProvisioningParameters .

              
            

            - **Value** *(string) --* 

              The desired value for this key.

              
        
      
    

  .. py:method:: create_portfolio_share(**kwargs)

    

    Creates a new portfolio share.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/CreatePortfolioShare>`_    


    **Request Syntax** 
    ::

      response = client.create_portfolio_share(
          AcceptLanguage='string',
          PortfolioId='string',
          AccountId='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type PortfolioId: string
    :param PortfolioId: **[REQUIRED]** 

      The portfolio identifier.

      

    
    :type AccountId: string
    :param AccountId: **[REQUIRED]** 

      The account ID with which to share the portfolio.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {}
        
      **Response Structure** 

      

      - *(dict) --* 
    

  .. py:method:: create_product(**kwargs)

    

    Creates a new product.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/CreateProduct>`_    


    **Request Syntax** 
    ::

      response = client.create_product(
          AcceptLanguage='string',
          Name='string',
          Owner='string',
          Description='string',
          Distributor='string',
          SupportDescription='string',
          SupportEmail='string',
          SupportUrl='string',
          ProductType='CLOUD_FORMATION_TEMPLATE'|'MARKETPLACE',
          Tags=[
              {
                  'Key': 'string',
                  'Value': 'string'
              },
          ],
          ProvisioningArtifactParameters={
              'Name': 'string',
              'Description': 'string',
              'Info': {
                  'string': 'string'
              },
              'Type': 'CLOUD_FORMATION_TEMPLATE'|'MARKETPLACE_AMI'|'MARKETPLACE_CAR'
          },
          IdempotencyToken='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type Name: string
    :param Name: **[REQUIRED]** 

      The name of the product.

      

    
    :type Owner: string
    :param Owner: **[REQUIRED]** 

      The owner of the product.

      

    
    :type Description: string
    :param Description: 

      The text description of the product.

      

    
    :type Distributor: string
    :param Distributor: 

      The distributor of the product.

      

    
    :type SupportDescription: string
    :param SupportDescription: 

      Support information about the product.

      

    
    :type SupportEmail: string
    :param SupportEmail: 

      Contact email for product support.

      

    
    :type SupportUrl: string
    :param SupportUrl: 

      Contact URL for product support.

      

    
    :type ProductType: string
    :param ProductType: **[REQUIRED]** 

      The type of the product to create.

      

    
    :type Tags: list
    :param Tags: 

      Tags to associate with the new product.

      

    
      - *(dict) --* 

        Key-value pairs to associate with this provisioning. These tags are entirely discretionary and are propagated to the resources created in the provisioning.

        

      
        - **Key** *(string) --* **[REQUIRED]** 

          The ``ProvisioningArtifactParameter.TagKey`` parameter from  DescribeProvisioningParameters .

          

        
        - **Value** *(string) --* **[REQUIRED]** 

          The desired value for this key.

          

        
      
  
    :type ProvisioningArtifactParameters: dict
    :param ProvisioningArtifactParameters: **[REQUIRED]** 

      Parameters for the provisioning artifact.

      

    
      - **Name** *(string) --* 

        The name assigned to the provisioning artifact properties.

        

      
      - **Description** *(string) --* 

        The text description of the provisioning artifact properties.

        

      
      - **Info** *(dict) --* **[REQUIRED]** 

        Additional information about the provisioning artifact properties. When using this element in a request, you must specify ``LoadTemplateFromURL`` . For more information, see  CreateProvisioningArtifact .

        

      
        - *(string) --* 

        
          - *(string) --* 

          
    
  
      - **Type** *(string) --* 

        The type of the provisioning artifact properties. The following provisioning artifact property types are used by AWS Marketplace products:

         

         ``MARKETPLACE_AMI`` - AMI products.

         

         ``MARKETPLACE_CAR`` - CAR (Cluster and AWS Resources) products.

        

      
    
    :type IdempotencyToken: string
    :param IdempotencyToken: **[REQUIRED]** 

      A token to disambiguate duplicate requests. You can use the same input in multiple requests, provided that you also specify a different idempotency token for each request.

      This field is autopopulated if not provided.

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ProductViewDetail': {
                'ProductViewSummary': {
                    'Id': 'string',
                    'ProductId': 'string',
                    'Name': 'string',
                    'Owner': 'string',
                    'ShortDescription': 'string',
                    'Type': 'CLOUD_FORMATION_TEMPLATE'|'MARKETPLACE',
                    'Distributor': 'string',
                    'HasDefaultPath': True|False,
                    'SupportEmail': 'string',
                    'SupportDescription': 'string',
                    'SupportUrl': 'string'
                },
                'Status': 'AVAILABLE'|'CREATING'|'FAILED',
                'ProductARN': 'string',
                'CreatedTime': datetime(2015, 1, 1)
            },
            'ProvisioningArtifactDetail': {
                'Id': 'string',
                'Name': 'string',
                'Description': 'string',
                'Type': 'CLOUD_FORMATION_TEMPLATE'|'MARKETPLACE_AMI'|'MARKETPLACE_CAR',
                'CreatedTime': datetime(2015, 1, 1)
            },
            'Tags': [
                {
                    'Key': 'string',
                    'Value': 'string'
                },
            ]
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ProductViewDetail** *(dict) --* 

          The resulting detailed product view information.

          
          

          - **ProductViewSummary** *(dict) --* 

            The summary metadata about the specified product view.

            
            

            - **Id** *(string) --* 

              The product view identifier.

              
            

            - **ProductId** *(string) --* 

              The product identifier.

              
            

            - **Name** *(string) --* 

              The name of the product.

              
            

            - **Owner** *(string) --* 

              The owner of the product. Contact the product administrator for the significance of this value.

              
            

            - **ShortDescription** *(string) --* 

              Short description of the product.

              
            

            - **Type** *(string) --* 

              The product type. Contact the product administrator for the significance of this value. If this value is ``MARKETPLACE`` , the product was created by AWS Marketplace.

              
            

            - **Distributor** *(string) --* 

              The distributor of the product. Contact the product administrator for the significance of this value.

              
            

            - **HasDefaultPath** *(boolean) --* 

              A value of ``false`` indicates that the product does not have a default path, while a value of ``true`` indicates that it does. If it's false, call  ListLaunchPaths to disambiguate between paths. If true,  ListLaunchPaths is not required, and the output of the  ProductViewSummary operation can be used directly with  DescribeProvisioningParameters .

              
            

            - **SupportEmail** *(string) --* 

              The email contact information to obtain support for this Product.

              
            

            - **SupportDescription** *(string) --* 

              The description of the support for this Product.

              
            

            - **SupportUrl** *(string) --* 

              The URL information to obtain support for this Product.

              
        
          

          - **Status** *(string) --* 

            Current status of the product.

             

             ``AVAILABLE`` - Product is available for use.

             

             ``CREATING`` - Creation of product started, not ready for use.

             

             ``FAILED`` - Action on product failed.

            
          

          - **ProductARN** *(string) --* 

            The ARN associated with the product.

            
          

          - **CreatedTime** *(datetime) --* 

            The UTC timestamp of the creation time.

            
      
        

        - **ProvisioningArtifactDetail** *(dict) --* 

          The resulting detailed provisioning artifact information.

          
          

          - **Id** *(string) --* 

            The identifier of the provisioning artifact. This is sometimes referred to as the product version.

            
          

          - **Name** *(string) --* 

            The name assigned to the provisioning artifact.

            
          

          - **Description** *(string) --* 

            The text description of the provisioning artifact.

            
          

          - **Type** *(string) --* 

            The type of the provisioning artifact. The following provisioning artifact types are used by AWS Marketplace products:

             

             ``MARKETPLACE_AMI`` - AMI products.

             

             ``MARKETPLACE_CAR`` - CAR (Cluster and AWS Resources) products.

            
          

          - **CreatedTime** *(datetime) --* 

            The UTC timestamp of the creation time.

            
      
        

        - **Tags** *(list) --* 

          Tags successfully associated with the new product.

          
          

          - *(dict) --* 

            Key-value pairs to associate with this provisioning. These tags are entirely discretionary and are propagated to the resources created in the provisioning.

            
            

            - **Key** *(string) --* 

              The ``ProvisioningArtifactParameter.TagKey`` parameter from  DescribeProvisioningParameters .

              
            

            - **Value** *(string) --* 

              The desired value for this key.

              
        
      
    

  .. py:method:: create_provisioning_artifact(**kwargs)

    

    Create a new provisioning artifact for the specified product. This operation does not work with a product that has been shared with you.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/CreateProvisioningArtifact>`_    


    **Request Syntax** 
    ::

      response = client.create_provisioning_artifact(
          AcceptLanguage='string',
          ProductId='string',
          Parameters={
              'Name': 'string',
              'Description': 'string',
              'Info': {
                  'string': 'string'
              },
              'Type': 'CLOUD_FORMATION_TEMPLATE'|'MARKETPLACE_AMI'|'MARKETPLACE_CAR'
          },
          IdempotencyToken='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type ProductId: string
    :param ProductId: **[REQUIRED]** 

      The product identifier.

      

    
    :type Parameters: dict
    :param Parameters: **[REQUIRED]** 

      The parameters to use when creating the new provisioning artifact.

      

    
      - **Name** *(string) --* 

        The name assigned to the provisioning artifact properties.

        

      
      - **Description** *(string) --* 

        The text description of the provisioning artifact properties.

        

      
      - **Info** *(dict) --* **[REQUIRED]** 

        Additional information about the provisioning artifact properties. When using this element in a request, you must specify ``LoadTemplateFromURL`` . For more information, see  CreateProvisioningArtifact .

        

      
        - *(string) --* 

        
          - *(string) --* 

          
    
  
      - **Type** *(string) --* 

        The type of the provisioning artifact properties. The following provisioning artifact property types are used by AWS Marketplace products:

         

         ``MARKETPLACE_AMI`` - AMI products.

         

         ``MARKETPLACE_CAR`` - CAR (Cluster and AWS Resources) products.

        

      
    
    :type IdempotencyToken: string
    :param IdempotencyToken: **[REQUIRED]** 

      A token to disambiguate duplicate requests. You can use the same input in multiple requests, provided that you also specify a different idempotency token for each request.

      This field is autopopulated if not provided.

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ProvisioningArtifactDetail': {
                'Id': 'string',
                'Name': 'string',
                'Description': 'string',
                'Type': 'CLOUD_FORMATION_TEMPLATE'|'MARKETPLACE_AMI'|'MARKETPLACE_CAR',
                'CreatedTime': datetime(2015, 1, 1)
            },
            'Info': {
                'string': 'string'
            },
            'Status': 'AVAILABLE'|'CREATING'|'FAILED'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ProvisioningArtifactDetail** *(dict) --* 

          The resulting detailed provisioning artifact information.

          
          

          - **Id** *(string) --* 

            The identifier of the provisioning artifact. This is sometimes referred to as the product version.

            
          

          - **Name** *(string) --* 

            The name assigned to the provisioning artifact.

            
          

          - **Description** *(string) --* 

            The text description of the provisioning artifact.

            
          

          - **Type** *(string) --* 

            The type of the provisioning artifact. The following provisioning artifact types are used by AWS Marketplace products:

             

             ``MARKETPLACE_AMI`` - AMI products.

             

             ``MARKETPLACE_CAR`` - CAR (Cluster and AWS Resources) products.

            
          

          - **CreatedTime** *(datetime) --* 

            The UTC timestamp of the creation time.

            
      
        

        - **Info** *(dict) --* 

          Additional information about the creation request for the provisioning artifact.

          
          

          - *(string) --* 
            

            - *(string) --* 
      
    
        

        - **Status** *(string) --* 

          The status of the current request.

          
    

  .. py:method:: create_tag_option(**kwargs)

    

    Create a new TagOption.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/CreateTagOption>`_    


    **Request Syntax** 
    ::

      response = client.create_tag_option(
          Key='string',
          Value='string'
      )
    :type Key: string
    :param Key: **[REQUIRED]** 

      The TagOption key.

      

    
    :type Value: string
    :param Value: **[REQUIRED]** 

      The TagOption value.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'TagOptionDetail': {
                'Key': 'string',
                'Value': 'string',
                'Active': True|False,
                'Id': 'string'
            }
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **TagOptionDetail** *(dict) --* 

          The resulting detailed TagOption information.

          
          

          - **Key** *(string) --* 

            The TagOptionDetail key.

            
          

          - **Value** *(string) --* 

            The TagOptionDetail value.

            
          

          - **Active** *(boolean) --* 

            The TagOptionDetail active state.

            
          

          - **Id** *(string) --* 

            The TagOptionDetail identifier.

            
      
    

  .. py:method:: delete_constraint(**kwargs)

    

    Deletes the specified constraint.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DeleteConstraint>`_    


    **Request Syntax** 
    ::

      response = client.delete_constraint(
          AcceptLanguage='string',
          Id='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type Id: string
    :param Id: **[REQUIRED]** 

      The identifier of the constraint to delete.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {}
        
      **Response Structure** 

      

      - *(dict) --* 
    

  .. py:method:: delete_portfolio(**kwargs)

    

    Deletes the specified portfolio. This operation does not work with a portfolio that has been shared with you or if it has products, users, constraints, or shared accounts associated with it.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DeletePortfolio>`_    


    **Request Syntax** 
    ::

      response = client.delete_portfolio(
          AcceptLanguage='string',
          Id='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type Id: string
    :param Id: **[REQUIRED]** 

      The identifier of the portfolio for the delete request.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {}
        
      **Response Structure** 

      

      - *(dict) --* 
    

  .. py:method:: delete_portfolio_share(**kwargs)

    

    Deletes the specified portfolio share.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DeletePortfolioShare>`_    


    **Request Syntax** 
    ::

      response = client.delete_portfolio_share(
          AcceptLanguage='string',
          PortfolioId='string',
          AccountId='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type PortfolioId: string
    :param PortfolioId: **[REQUIRED]** 

      The portfolio identifier.

      

    
    :type AccountId: string
    :param AccountId: **[REQUIRED]** 

      The account ID associated with the share to delete.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {}
        
      **Response Structure** 

      

      - *(dict) --* 
    

  .. py:method:: delete_product(**kwargs)

    

    Deletes the specified product. This operation does not work with a product that has been shared with you or is associated with a portfolio. 

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DeleteProduct>`_    


    **Request Syntax** 
    ::

      response = client.delete_product(
          AcceptLanguage='string',
          Id='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type Id: string
    :param Id: **[REQUIRED]** 

      The identifier of the product for the delete request.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {}
        
      **Response Structure** 

      

      - *(dict) --* 
    

  .. py:method:: delete_provisioning_artifact(**kwargs)

    

    Deletes the specified provisioning artifact. This operation does not work on a provisioning artifact associated with a product that has been shared with you, or on the last provisioning artifact associated with a product (a product must have at least one provisioning artifact).

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DeleteProvisioningArtifact>`_    


    **Request Syntax** 
    ::

      response = client.delete_provisioning_artifact(
          AcceptLanguage='string',
          ProductId='string',
          ProvisioningArtifactId='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type ProductId: string
    :param ProductId: **[REQUIRED]** 

      The product identifier.

      

    
    :type ProvisioningArtifactId: string
    :param ProvisioningArtifactId: **[REQUIRED]** 

      The identifier of the provisioning artifact for the delete request. This is sometimes referred to as the product version.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {}
        
      **Response Structure** 

      

      - *(dict) --* 
    

  .. py:method:: describe_constraint(**kwargs)

    

    Retrieves detailed information for a specified constraint.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DescribeConstraint>`_    


    **Request Syntax** 
    ::

      response = client.describe_constraint(
          AcceptLanguage='string',
          Id='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type Id: string
    :param Id: **[REQUIRED]** 

      The identifier of the constraint.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ConstraintDetail': {
                'ConstraintId': 'string',
                'Type': 'string',
                'Description': 'string',
                'Owner': 'string'
            },
            'ConstraintParameters': 'string',
            'Status': 'AVAILABLE'|'CREATING'|'FAILED'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ConstraintDetail** *(dict) --* 

          Detailed constraint information.

          
          

          - **ConstraintId** *(string) --* 

            The identifier of the constraint.

            
          

          - **Type** *(string) --* 

            The type of the constraint.

            
          

          - **Description** *(string) --* 

            The text description of the constraint.

            
          

          - **Owner** *(string) --* 

            The owner of the constraint.

            
      
        

        - **ConstraintParameters** *(string) --* 

          The current parameters associated with the specified constraint.

          
        

        - **Status** *(string) --* 

          The status of the current request.

          
    

  .. py:method:: describe_copy_product_status(**kwargs)

    

    Describes the status of the specified copy product operation.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DescribeCopyProductStatus>`_    


    **Request Syntax** 
    ::

      response = client.describe_copy_product_status(
          AcceptLanguage='string',
          CopyProductToken='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type CopyProductToken: string
    :param CopyProductToken: **[REQUIRED]** 

      The token returned from the call to ``CopyProduct`` that initiated the operation.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'CopyProductStatus': 'SUCCEEDED'|'IN_PROGRESS'|'FAILED',
            'TargetProductId': 'string',
            'StatusDetail': 'string'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **CopyProductStatus** *(string) --* 

          The status of the copy product operation.

          
        

        - **TargetProductId** *(string) --* 

          The ID of the copied product.

          
        

        - **StatusDetail** *(string) --* 

          The status message.

          
    

  .. py:method:: describe_portfolio(**kwargs)

    

    Retrieves detailed information and any tags associated with the specified portfolio.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DescribePortfolio>`_    


    **Request Syntax** 
    ::

      response = client.describe_portfolio(
          AcceptLanguage='string',
          Id='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type Id: string
    :param Id: **[REQUIRED]** 

      The identifier of the portfolio for which to retrieve information.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'PortfolioDetail': {
                'Id': 'string',
                'ARN': 'string',
                'DisplayName': 'string',
                'Description': 'string',
                'CreatedTime': datetime(2015, 1, 1),
                'ProviderName': 'string'
            },
            'Tags': [
                {
                    'Key': 'string',
                    'Value': 'string'
                },
            ],
            'TagOptions': [
                {
                    'Key': 'string',
                    'Value': 'string',
                    'Active': True|False,
                    'Id': 'string'
                },
            ]
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **PortfolioDetail** *(dict) --* 

          Detailed portfolio information.

          
          

          - **Id** *(string) --* 

            The identifier for the portfolio.

            
          

          - **ARN** *(string) --* 

            The ARN assigned to the portfolio.

            
          

          - **DisplayName** *(string) --* 

            The name to use for display purposes.

            
          

          - **Description** *(string) --* 

            The text description of the portfolio.

            
          

          - **CreatedTime** *(datetime) --* 

            The UTC timestamp of the creation time.

            
          

          - **ProviderName** *(string) --* 

            The name of the portfolio provider.

            
      
        

        - **Tags** *(list) --* 

          Tags associated with the portfolio.

          
          

          - *(dict) --* 

            Key-value pairs to associate with this provisioning. These tags are entirely discretionary and are propagated to the resources created in the provisioning.

            
            

            - **Key** *(string) --* 

              The ``ProvisioningArtifactParameter.TagKey`` parameter from  DescribeProvisioningParameters .

              
            

            - **Value** *(string) --* 

              The desired value for this key.

              
        
      
        

        - **TagOptions** *(list) --* 

          TagOptions associated with the portfolio.

          
          

          - *(dict) --* 

            The TagOption details.

            
            

            - **Key** *(string) --* 

              The TagOptionDetail key.

              
            

            - **Value** *(string) --* 

              The TagOptionDetail value.

              
            

            - **Active** *(boolean) --* 

              The TagOptionDetail active state.

              
            

            - **Id** *(string) --* 

              The TagOptionDetail identifier.

              
        
      
    

  .. py:method:: describe_product(**kwargs)

    

    Retrieves information about a specified product.

     

    This operation is functionally identical to  DescribeProductView except that it takes as input ``ProductId`` instead of ``ProductViewId`` .

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DescribeProduct>`_    


    **Request Syntax** 
    ::

      response = client.describe_product(
          AcceptLanguage='string',
          Id='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type Id: string
    :param Id: **[REQUIRED]** 

      The ``ProductId`` of the product to describe.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ProductViewSummary': {
                'Id': 'string',
                'ProductId': 'string',
                'Name': 'string',
                'Owner': 'string',
                'ShortDescription': 'string',
                'Type': 'CLOUD_FORMATION_TEMPLATE'|'MARKETPLACE',
                'Distributor': 'string',
                'HasDefaultPath': True|False,
                'SupportEmail': 'string',
                'SupportDescription': 'string',
                'SupportUrl': 'string'
            },
            'ProvisioningArtifacts': [
                {
                    'Id': 'string',
                    'Name': 'string',
                    'Description': 'string',
                    'CreatedTime': datetime(2015, 1, 1)
                },
            ]
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ProductViewSummary** *(dict) --* 

          The summary metadata about the specified product.

          
          

          - **Id** *(string) --* 

            The product view identifier.

            
          

          - **ProductId** *(string) --* 

            The product identifier.

            
          

          - **Name** *(string) --* 

            The name of the product.

            
          

          - **Owner** *(string) --* 

            The owner of the product. Contact the product administrator for the significance of this value.

            
          

          - **ShortDescription** *(string) --* 

            Short description of the product.

            
          

          - **Type** *(string) --* 

            The product type. Contact the product administrator for the significance of this value. If this value is ``MARKETPLACE`` , the product was created by AWS Marketplace.

            
          

          - **Distributor** *(string) --* 

            The distributor of the product. Contact the product administrator for the significance of this value.

            
          

          - **HasDefaultPath** *(boolean) --* 

            A value of ``false`` indicates that the product does not have a default path, while a value of ``true`` indicates that it does. If it's false, call  ListLaunchPaths to disambiguate between paths. If true,  ListLaunchPaths is not required, and the output of the  ProductViewSummary operation can be used directly with  DescribeProvisioningParameters .

            
          

          - **SupportEmail** *(string) --* 

            The email contact information to obtain support for this Product.

            
          

          - **SupportDescription** *(string) --* 

            The description of the support for this Product.

            
          

          - **SupportUrl** *(string) --* 

            The URL information to obtain support for this Product.

            
      
        

        - **ProvisioningArtifacts** *(list) --* 

          A list of provisioning artifact objects for the specified product. The ``ProvisioningArtifacts`` parameter represent the ways the specified product can be provisioned.

          
          

          - *(dict) --* 

            Contains information indicating the ways in which a product can be provisioned.

            
            

            - **Id** *(string) --* 

              The identifier for the artifact. This is sometimes referred to as the product version.

              
            

            - **Name** *(string) --* 

              The name of the artifact.

              
            

            - **Description** *(string) --* 

              The text description of the artifact.

              
            

            - **CreatedTime** *(datetime) --* 

              The UTC timestamp of the creation time.

              
        
      
    

  .. py:method:: describe_product_as_admin(**kwargs)

    

    Retrieves information about a specified product, run with administrator access.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DescribeProductAsAdmin>`_    


    **Request Syntax** 
    ::

      response = client.describe_product_as_admin(
          AcceptLanguage='string',
          Id='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type Id: string
    :param Id: **[REQUIRED]** 

      The identifier of the product for which to retrieve information.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ProductViewDetail': {
                'ProductViewSummary': {
                    'Id': 'string',
                    'ProductId': 'string',
                    'Name': 'string',
                    'Owner': 'string',
                    'ShortDescription': 'string',
                    'Type': 'CLOUD_FORMATION_TEMPLATE'|'MARKETPLACE',
                    'Distributor': 'string',
                    'HasDefaultPath': True|False,
                    'SupportEmail': 'string',
                    'SupportDescription': 'string',
                    'SupportUrl': 'string'
                },
                'Status': 'AVAILABLE'|'CREATING'|'FAILED',
                'ProductARN': 'string',
                'CreatedTime': datetime(2015, 1, 1)
            },
            'ProvisioningArtifactSummaries': [
                {
                    'Id': 'string',
                    'Name': 'string',
                    'Description': 'string',
                    'CreatedTime': datetime(2015, 1, 1),
                    'ProvisioningArtifactMetadata': {
                        'string': 'string'
                    }
                },
            ],
            'Tags': [
                {
                    'Key': 'string',
                    'Value': 'string'
                },
            ],
            'TagOptions': [
                {
                    'Key': 'string',
                    'Value': 'string',
                    'Active': True|False,
                    'Id': 'string'
                },
            ]
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ProductViewDetail** *(dict) --* 

          Detailed product view information.

          
          

          - **ProductViewSummary** *(dict) --* 

            The summary metadata about the specified product view.

            
            

            - **Id** *(string) --* 

              The product view identifier.

              
            

            - **ProductId** *(string) --* 

              The product identifier.

              
            

            - **Name** *(string) --* 

              The name of the product.

              
            

            - **Owner** *(string) --* 

              The owner of the product. Contact the product administrator for the significance of this value.

              
            

            - **ShortDescription** *(string) --* 

              Short description of the product.

              
            

            - **Type** *(string) --* 

              The product type. Contact the product administrator for the significance of this value. If this value is ``MARKETPLACE`` , the product was created by AWS Marketplace.

              
            

            - **Distributor** *(string) --* 

              The distributor of the product. Contact the product administrator for the significance of this value.

              
            

            - **HasDefaultPath** *(boolean) --* 

              A value of ``false`` indicates that the product does not have a default path, while a value of ``true`` indicates that it does. If it's false, call  ListLaunchPaths to disambiguate between paths. If true,  ListLaunchPaths is not required, and the output of the  ProductViewSummary operation can be used directly with  DescribeProvisioningParameters .

              
            

            - **SupportEmail** *(string) --* 

              The email contact information to obtain support for this Product.

              
            

            - **SupportDescription** *(string) --* 

              The description of the support for this Product.

              
            

            - **SupportUrl** *(string) --* 

              The URL information to obtain support for this Product.

              
        
          

          - **Status** *(string) --* 

            Current status of the product.

             

             ``AVAILABLE`` - Product is available for use.

             

             ``CREATING`` - Creation of product started, not ready for use.

             

             ``FAILED`` - Action on product failed.

            
          

          - **ProductARN** *(string) --* 

            The ARN associated with the product.

            
          

          - **CreatedTime** *(datetime) --* 

            The UTC timestamp of the creation time.

            
      
        

        - **ProvisioningArtifactSummaries** *(list) --* 

          A list of provisioning artifact summaries for the product.

          
          

          - *(dict) --* 

            Stores summary information about a provisioning artifact.

            
            

            - **Id** *(string) --* 

              The identifier of the provisioning artifact.

              
            

            - **Name** *(string) --* 

              The name of the provisioning artifact.

              
            

            - **Description** *(string) --* 

              The description of the provisioning artifact.

              
            

            - **CreatedTime** *(datetime) --* 

              The UTC timestamp of the creation time.

              
            

            - **ProvisioningArtifactMetadata** *(dict) --* 

              The provisioning artifact metadata. This data is used with products created by AWS Marketplace.

              
              

              - *(string) --* 
                

                - *(string) --* 
          
        
        
      
        

        - **Tags** *(list) --* 

          Tags associated with the product.

          
          

          - *(dict) --* 

            Key-value pairs to associate with this provisioning. These tags are entirely discretionary and are propagated to the resources created in the provisioning.

            
            

            - **Key** *(string) --* 

              The ``ProvisioningArtifactParameter.TagKey`` parameter from  DescribeProvisioningParameters .

              
            

            - **Value** *(string) --* 

              The desired value for this key.

              
        
      
        

        - **TagOptions** *(list) --* 

          List of TagOptions associated with the product.

          
          

          - *(dict) --* 

            The TagOption details.

            
            

            - **Key** *(string) --* 

              The TagOptionDetail key.

              
            

            - **Value** *(string) --* 

              The TagOptionDetail value.

              
            

            - **Active** *(boolean) --* 

              The TagOptionDetail active state.

              
            

            - **Id** *(string) --* 

              The TagOptionDetail identifier.

              
        
      
    

  .. py:method:: describe_product_view(**kwargs)

    

    Retrieves information about a specified product.

     

    This operation is functionally identical to  DescribeProduct except that it takes as input ``ProductViewId`` instead of ``ProductId`` .

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DescribeProductView>`_    


    **Request Syntax** 
    ::

      response = client.describe_product_view(
          AcceptLanguage='string',
          Id='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type Id: string
    :param Id: **[REQUIRED]** 

      The ``ProductViewId`` of the product to describe.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ProductViewSummary': {
                'Id': 'string',
                'ProductId': 'string',
                'Name': 'string',
                'Owner': 'string',
                'ShortDescription': 'string',
                'Type': 'CLOUD_FORMATION_TEMPLATE'|'MARKETPLACE',
                'Distributor': 'string',
                'HasDefaultPath': True|False,
                'SupportEmail': 'string',
                'SupportDescription': 'string',
                'SupportUrl': 'string'
            },
            'ProvisioningArtifacts': [
                {
                    'Id': 'string',
                    'Name': 'string',
                    'Description': 'string',
                    'CreatedTime': datetime(2015, 1, 1)
                },
            ]
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ProductViewSummary** *(dict) --* 

          The summary metadata about the specified product.

          
          

          - **Id** *(string) --* 

            The product view identifier.

            
          

          - **ProductId** *(string) --* 

            The product identifier.

            
          

          - **Name** *(string) --* 

            The name of the product.

            
          

          - **Owner** *(string) --* 

            The owner of the product. Contact the product administrator for the significance of this value.

            
          

          - **ShortDescription** *(string) --* 

            Short description of the product.

            
          

          - **Type** *(string) --* 

            The product type. Contact the product administrator for the significance of this value. If this value is ``MARKETPLACE`` , the product was created by AWS Marketplace.

            
          

          - **Distributor** *(string) --* 

            The distributor of the product. Contact the product administrator for the significance of this value.

            
          

          - **HasDefaultPath** *(boolean) --* 

            A value of ``false`` indicates that the product does not have a default path, while a value of ``true`` indicates that it does. If it's false, call  ListLaunchPaths to disambiguate between paths. If true,  ListLaunchPaths is not required, and the output of the  ProductViewSummary operation can be used directly with  DescribeProvisioningParameters .

            
          

          - **SupportEmail** *(string) --* 

            The email contact information to obtain support for this Product.

            
          

          - **SupportDescription** *(string) --* 

            The description of the support for this Product.

            
          

          - **SupportUrl** *(string) --* 

            The URL information to obtain support for this Product.

            
      
        

        - **ProvisioningArtifacts** *(list) --* 

          A list of provisioning artifact objects for the specified product. The ``ProvisioningArtifacts`` represent the ways in which the specified product can be provisioned.

          
          

          - *(dict) --* 

            Contains information indicating the ways in which a product can be provisioned.

            
            

            - **Id** *(string) --* 

              The identifier for the artifact. This is sometimes referred to as the product version.

              
            

            - **Name** *(string) --* 

              The name of the artifact.

              
            

            - **Description** *(string) --* 

              The text description of the artifact.

              
            

            - **CreatedTime** *(datetime) --* 

              The UTC timestamp of the creation time.

              
        
      
    

  .. py:method:: describe_provisioned_product(**kwargs)

    

    Retrieve detailed information about the provisioned product.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DescribeProvisionedProduct>`_    


    **Request Syntax** 
    ::

      response = client.describe_provisioned_product(
          AcceptLanguage='string',
          Id='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type Id: string
    :param Id: **[REQUIRED]** 

      The provisioned product identifier.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ProvisionedProductDetail': {
                'Name': 'string',
                'Arn': 'string',
                'Type': 'string',
                'Id': 'string',
                'Status': 'AVAILABLE'|'UNDER_CHANGE'|'TAINTED'|'ERROR',
                'StatusMessage': 'string',
                'CreatedTime': datetime(2015, 1, 1),
                'IdempotencyToken': 'string',
                'LastRecordId': 'string'
            }
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ProvisionedProductDetail** *(dict) --* 

          Detailed provisioned product information.

          
          

          - **Name** *(string) --* 

            The user-friendly name of the ProvisionedProduct object.

            
          

          - **Arn** *(string) --* 

            The ARN associated with the ProvisionedProduct object.

            
          

          - **Type** *(string) --* 

            The type of the ProvisionedProduct object.

            
          

          - **Id** *(string) --* 

            The identifier of the ProvisionedProduct object.

            
          

          - **Status** *(string) --* 

            The current status of the ProvisionedProduct.

             

             ``AVAILABLE`` - Stable state, ready to perform any operation. The most recent action request succeeded and completed.

             

             ``UNDER_CHANGE`` - Transitive state, operations performed may or may not have valid results. Wait for an ``AVAILABLE`` status before performing operations.

             

             ``TAINTED`` - Stable state, ready to perform any operation. The stack has completed the requested operation but is not exactly what was requested. For example, a request to update to a new version failed and the stack rolled back to the current version. 

             

             ``ERROR`` - Something unexpected happened such that the provisioned product exists but the stack is not running. For example, CloudFormation received an invalid parameter value and could not launch the stack.

            
          

          - **StatusMessage** *(string) --* 

            The current status message of the ProvisionedProduct.

            
          

          - **CreatedTime** *(datetime) --* 

            The UTC timestamp of the creation time.

            
          

          - **IdempotencyToken** *(string) --* 

            A token to disambiguate duplicate requests. You can use the same input in multiple requests, provided that you also specify a different idempotency token for each request.

            
          

          - **LastRecordId** *(string) --* 

            The record identifier of the last request performed on this ProvisionedProduct object.

            
      
    

  .. py:method:: describe_provisioning_artifact(**kwargs)

    

    Retrieves detailed information about the specified provisioning artifact.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DescribeProvisioningArtifact>`_    


    **Request Syntax** 
    ::

      response = client.describe_provisioning_artifact(
          AcceptLanguage='string',
          ProvisioningArtifactId='string',
          ProductId='string',
          Verbose=True|False
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type ProvisioningArtifactId: string
    :param ProvisioningArtifactId: **[REQUIRED]** 

      The identifier of the provisioning artifact. This is sometimes referred to as the product version.

      

    
    :type ProductId: string
    :param ProductId: **[REQUIRED]** 

      The product identifier.

      

    
    :type Verbose: boolean
    :param Verbose: 

      Enable a verbose level of details for the provisioning artifact.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ProvisioningArtifactDetail': {
                'Id': 'string',
                'Name': 'string',
                'Description': 'string',
                'Type': 'CLOUD_FORMATION_TEMPLATE'|'MARKETPLACE_AMI'|'MARKETPLACE_CAR',
                'CreatedTime': datetime(2015, 1, 1)
            },
            'Info': {
                'string': 'string'
            },
            'Status': 'AVAILABLE'|'CREATING'|'FAILED'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ProvisioningArtifactDetail** *(dict) --* 

          Detailed provisioning artifact information.

          
          

          - **Id** *(string) --* 

            The identifier of the provisioning artifact. This is sometimes referred to as the product version.

            
          

          - **Name** *(string) --* 

            The name assigned to the provisioning artifact.

            
          

          - **Description** *(string) --* 

            The text description of the provisioning artifact.

            
          

          - **Type** *(string) --* 

            The type of the provisioning artifact. The following provisioning artifact types are used by AWS Marketplace products:

             

             ``MARKETPLACE_AMI`` - AMI products.

             

             ``MARKETPLACE_CAR`` - CAR (Cluster and AWS Resources) products.

            
          

          - **CreatedTime** *(datetime) --* 

            The UTC timestamp of the creation time.

            
      
        

        - **Info** *(dict) --* 

          Additional information about the provisioning artifact.

          
          

          - *(string) --* 
            

            - *(string) --* 
      
    
        

        - **Status** *(string) --* 

          The status of the current request.

          
    

  .. py:method:: describe_provisioning_parameters(**kwargs)

    

    Provides information about parameters required to provision a specified product in a specified manner. Use this operation to obtain the list of ``ProvisioningArtifactParameters`` parameters available to call the  ProvisionProduct operation for the specified product.

     

    If the output contains a TagOption key with an empty list of values, there is a TagOption conflict for that key. The end user cannot take action to fix the conflict, and launch is not blocked. In subsequent calls to the ``ProvisionProduct`` operation, do not include conflicted TagOption keys as tags. Calls to ``ProvisionProduct`` with empty TagOption values cause the error "Parameter validation failed: Missing required parameter in Tags[*N* ]:*Value* ". Calls to ``ProvisionProduct`` with conflicted TagOption keys automatically tag the provisioned product with the conflicted keys with the value "``sc-tagoption-conflict-portfolioId-productId`` ".

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DescribeProvisioningParameters>`_    


    **Request Syntax** 
    ::

      response = client.describe_provisioning_parameters(
          AcceptLanguage='string',
          ProductId='string',
          ProvisioningArtifactId='string',
          PathId='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type ProductId: string
    :param ProductId: **[REQUIRED]** 

      The product identifier.

      

    
    :type ProvisioningArtifactId: string
    :param ProvisioningArtifactId: **[REQUIRED]** 

      The provisioning artifact identifier for this product. This is sometimes referred to as the product version.

      

    
    :type PathId: string
    :param PathId: 

      The identifier of the path for this product's provisioning. This value is optional if the product has a default path, and is required if there is more than one path for the specified product.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ProvisioningArtifactParameters': [
                {
                    'ParameterKey': 'string',
                    'DefaultValue': 'string',
                    'ParameterType': 'string',
                    'IsNoEcho': True|False,
                    'Description': 'string',
                    'ParameterConstraints': {
                        'AllowedValues': [
                            'string',
                        ]
                    }
                },
            ],
            'ConstraintSummaries': [
                {
                    'Type': 'string',
                    'Description': 'string'
                },
            ],
            'UsageInstructions': [
                {
                    'Type': 'string',
                    'Value': 'string'
                },
            ],
            'TagOptions': [
                {
                    'Key': 'string',
                    'Values': [
                        'string',
                    ]
                },
            ]
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ProvisioningArtifactParameters** *(list) --* 

          The list of parameters used to successfully provision the product. Each parameter includes a list of allowable values and additional metadata about each parameter.

          
          

          - *(dict) --* 

            A parameter used to successfully provision the product. This value includes a list of allowable values and additional metadata. 

            
            

            - **ParameterKey** *(string) --* 

              The parameter key. 

              
            

            - **DefaultValue** *(string) --* 

              The default value for this parameter.

              
            

            - **ParameterType** *(string) --* 

              The parameter type.

              
            

            - **IsNoEcho** *(boolean) --* 

              If this value is true, the value for this parameter is obfuscated from view when the parameter is retrieved. This parameter is used to hide sensitive information.

              
            

            - **Description** *(string) --* 

              The text description of the parameter.

              
            

            - **ParameterConstraints** *(dict) --* 

              The list of constraints that the administrator has put on the parameter.

              
              

              - **AllowedValues** *(list) --* 

                The values that the administrator has allowed for the parameter.

                
                

                - *(string) --* 
            
          
        
      
        

        - **ConstraintSummaries** *(list) --* 

          The list of constraint summaries that apply to provisioning this product.

          
          

          - *(dict) --* 

            An administrator-specified constraint to apply when provisioning a product.

            
            

            - **Type** *(string) --* 

              The type of the constraint. 

              
            

            - **Description** *(string) --* 

              The text description of the constraint.

              
        
      
        

        - **UsageInstructions** *(list) --* 

          Any additional metadata specifically related to the provisioning of the product. For example, see the ``Version`` field of the CloudFormation template.

          
          

          - *(dict) --* 

            Additional information provided by the administrator.

            
            

            - **Type** *(string) --* 

              The usage instruction type for the value.

              
            

            - **Value** *(string) --* 

              The usage instruction value for this type.

              
        
      
        

        - **TagOptions** *(list) --* 

          List of TagOptions associated with the provisioned provisioning parameters.

          
          

          - *(dict) --* 

            The TagOption summary key-value pair.

            
            

            - **Key** *(string) --* 

              The TagOptionSummary key.

              
            

            - **Values** *(list) --* 

              The TagOptionSummary value.

              
              

              - *(string) --* 
          
        
      
    

  .. py:method:: describe_record(**kwargs)

    

    Retrieves a paginated list of the full details of a specific request. Use this operation after calling a request operation ( ProvisionProduct ,  TerminateProvisionedProduct , or  UpdateProvisionedProduct ). 

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DescribeRecord>`_    


    **Request Syntax** 
    ::

      response = client.describe_record(
          AcceptLanguage='string',
          Id='string',
          PageToken='string',
          PageSize=123
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type Id: string
    :param Id: **[REQUIRED]** 

      The record identifier of the ProvisionedProduct object for which to retrieve output information. This is the ``RecordDetail.RecordId`` obtained from the request operation's response.

      

    
    :type PageToken: string
    :param PageToken: 

      The page token of the first page retrieved. If null, this retrieves the first page of size ``PageSize`` .

      

    
    :type PageSize: integer
    :param PageSize: 

      The maximum number of items to return in the results. If more results exist than fit in the specified ``PageSize`` , the value of ``NextPageToken`` in the response is non-null.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'RecordDetail': {
                'RecordId': 'string',
                'ProvisionedProductName': 'string',
                'Status': 'CREATED'|'IN_PROGRESS'|'IN_PROGRESS_IN_ERROR'|'SUCCEEDED'|'FAILED',
                'CreatedTime': datetime(2015, 1, 1),
                'UpdatedTime': datetime(2015, 1, 1),
                'ProvisionedProductType': 'string',
                'RecordType': 'string',
                'ProvisionedProductId': 'string',
                'ProductId': 'string',
                'ProvisioningArtifactId': 'string',
                'PathId': 'string',
                'RecordErrors': [
                    {
                        'Code': 'string',
                        'Description': 'string'
                    },
                ],
                'RecordTags': [
                    {
                        'Key': 'string',
                        'Value': 'string'
                    },
                ]
            },
            'RecordOutputs': [
                {
                    'OutputKey': 'string',
                    'OutputValue': 'string',
                    'Description': 'string'
                },
            ],
            'NextPageToken': 'string'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **RecordDetail** *(dict) --* 

          Detailed record information for the specified product. 

          
          

          - **RecordId** *(string) --* 

            The identifier of the ProvisionedProduct object record.

            
          

          - **ProvisionedProductName** *(string) --* 

            The user-friendly name of the ProvisionedProduct object.

            
          

          - **Status** *(string) --* 

            The status of the ProvisionedProduct object.

             

             ``CREATED`` - Request created but the operation has not yet started.

             

             ``IN_PROGRESS`` - The requested operation is in-progress.

             

             ``IN_PROGRESS_IN_ERROR`` - The provisioned product is under change but the requested operation failed and some remediation is occurring. For example, a rollback.

             

             ``SUCCEEDED`` - The requested operation has successfully completed.

             

             ``FAILED`` - The requested operation has completed but has failed. Investigate using the error messages returned.

            
          

          - **CreatedTime** *(datetime) --* 

            The UTC timestamp of the creation time.

            
          

          - **UpdatedTime** *(datetime) --* 

            The time when the record for the ProvisionedProduct object was last updated.

            
          

          - **ProvisionedProductType** *(string) --* 

            The type of the ProvisionedProduct object.

            
          

          - **RecordType** *(string) --* 

            The record type for this record.

            
          

          - **ProvisionedProductId** *(string) --* 

            The identifier of the ProvisionedProduct object.

            
          

          - **ProductId** *(string) --* 

            The product identifier.

            
          

          - **ProvisioningArtifactId** *(string) --* 

            The provisioning artifact identifier for this product. This is sometimes referred to as the product version.

            
          

          - **PathId** *(string) --* 

            The identifier of the path for this product's provisioning.

            
          

          - **RecordErrors** *(list) --* 

            A list of errors that occurred while processing the request.

            
            

            - *(dict) --* 

              The error code and description resulting from an operation.

              
              

              - **Code** *(string) --* 

                The numeric value of the error.

                
              

              - **Description** *(string) --* 

                The text description of the error.

                
          
        
          

          - **RecordTags** *(list) --* 

            List of tags associated with this record.

            
            

            - *(dict) --* 

              A tag associated with the record, stored as a key-value pair.

              
              

              - **Key** *(string) --* 

                The key for this tag.

                
              

              - **Value** *(string) --* 

                The value for this tag.

                
          
        
      
        

        - **RecordOutputs** *(list) --* 

          A list of outputs for the specified Product object created as the result of a request. For example, a CloudFormation-backed product that creates an S3 bucket would have an output for the S3 bucket URL.

          
          

          - *(dict) --* 

            An output for the specified Product object created as the result of a request. For example, a CloudFormation-backed product that creates an S3 bucket would have an output for the S3 bucket URL.

            
            

            - **OutputKey** *(string) --* 

              The output key.

              
            

            - **OutputValue** *(string) --* 

              The output value.

              
            

            - **Description** *(string) --* 

              The text description of the output.

              
        
      
        

        - **NextPageToken** *(string) --* 

          The page token to use to retrieve the next page of results for this operation. If there are no more pages, this value is null.

          
    

  .. py:method:: describe_tag_option(**kwargs)

    

    Describes a TagOption.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DescribeTagOption>`_    


    **Request Syntax** 
    ::

      response = client.describe_tag_option(
          Id='string'
      )
    :type Id: string
    :param Id: **[REQUIRED]** 

      The identifier of the TagOption.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'TagOptionDetail': {
                'Key': 'string',
                'Value': 'string',
                'Active': True|False,
                'Id': 'string'
            }
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **TagOptionDetail** *(dict) --* 

          The resulting detailed TagOption information.

          
          

          - **Key** *(string) --* 

            The TagOptionDetail key.

            
          

          - **Value** *(string) --* 

            The TagOptionDetail value.

            
          

          - **Active** *(boolean) --* 

            The TagOptionDetail active state.

            
          

          - **Id** *(string) --* 

            The TagOptionDetail identifier.

            
      
    

  .. py:method:: disassociate_principal_from_portfolio(**kwargs)

    

    Disassociates a previously associated principal ARN from a specified portfolio.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DisassociatePrincipalFromPortfolio>`_    


    **Request Syntax** 
    ::

      response = client.disassociate_principal_from_portfolio(
          AcceptLanguage='string',
          PortfolioId='string',
          PrincipalARN='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type PortfolioId: string
    :param PortfolioId: **[REQUIRED]** 

      The portfolio identifier.

      

    
    :type PrincipalARN: string
    :param PrincipalARN: **[REQUIRED]** 

      The ARN representing the principal (IAM user, role, or group).

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {}
        
      **Response Structure** 

      

      - *(dict) --* 
    

  .. py:method:: disassociate_product_from_portfolio(**kwargs)

    

    Disassociates the specified product from the specified portfolio. 

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DisassociateProductFromPortfolio>`_    


    **Request Syntax** 
    ::

      response = client.disassociate_product_from_portfolio(
          AcceptLanguage='string',
          ProductId='string',
          PortfolioId='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type ProductId: string
    :param ProductId: **[REQUIRED]** 

      The product identifier.

      

    
    :type PortfolioId: string
    :param PortfolioId: **[REQUIRED]** 

      The portfolio identifier.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {}
        
      **Response Structure** 

      

      - *(dict) --* 
    

  .. py:method:: disassociate_tag_option_from_resource(**kwargs)

    

    Disassociates a TagOption from a resource.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/DisassociateTagOptionFromResource>`_    


    **Request Syntax** 
    ::

      response = client.disassociate_tag_option_from_resource(
          ResourceId='string',
          TagOptionId='string'
      )
    :type ResourceId: string
    :param ResourceId: **[REQUIRED]** 

      Identifier of the resource from which to disassociate the TagOption.

      

    
    :type TagOptionId: string
    :param TagOptionId: **[REQUIRED]** 

      Identifier of the TagOption to disassociate from the resource.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {}
        
      **Response Structure** 

      

      - *(dict) --* 
    

  .. py:method:: generate_presigned_url(ClientMethod, Params=None, ExpiresIn=3600, HttpMethod=None)

        
    Generate a presigned url given a client, its method, and arguments
    
    :type ClientMethod: string
    :param ClientMethod: The client method to presign for
    
    :type Params: dict
    :param Params: The parameters normally passed to
        ``ClientMethod``.
    
    :type ExpiresIn: int
    :param ExpiresIn: The number of seconds the presigned url is valid
        for. By default it expires in an hour (3600 seconds)
    
    :type HttpMethod: string
    :param HttpMethod: The http method to use on the generated url. By
        default, the http method is whatever is used in the method's model.
    
    :returns: The presigned url


  .. py:method:: get_paginator(operation_name)

        
    Create a paginator for an operation.
    
    :type operation_name: string
    :param operation_name: The operation name.  This is the same name
        as the method name on the client.  For example, if the
        method name is ``create_foo``, and you'd normally invoke the
        operation as ``client.create_foo(**kwargs)``, if the
        ``create_foo`` operation can be paginated, you can use the
        call ``client.get_paginator("create_foo")``.
    
    :raise OperationNotPageableError: Raised if the operation is not
        pageable.  You can use the ``client.can_paginate`` method to
        check if an operation is pageable.
    
    :rtype: L{botocore.paginate.Paginator}
    :return: A paginator object.


  .. py:method:: get_waiter(waiter_name)

        


  .. py:method:: list_accepted_portfolio_shares(**kwargs)

    

    Lists details of all portfolios for which sharing was accepted by this account.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/ListAcceptedPortfolioShares>`_    


    **Request Syntax** 
    ::

      response = client.list_accepted_portfolio_shares(
          AcceptLanguage='string',
          PageToken='string',
          PageSize=123
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type PageToken: string
    :param PageToken: 

      The page token of the first page retrieved. If null, this retrieves the first page of size ``PageSize`` .

      

    
    :type PageSize: integer
    :param PageSize: 

      The maximum number of items to return in the results. If more results exist than fit in the specified ``PageSize`` , the value of ``NextPageToken`` in the response is non-null.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'PortfolioDetails': [
                {
                    'Id': 'string',
                    'ARN': 'string',
                    'DisplayName': 'string',
                    'Description': 'string',
                    'CreatedTime': datetime(2015, 1, 1),
                    'ProviderName': 'string'
                },
            ],
            'NextPageToken': 'string'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **PortfolioDetails** *(list) --* 

          List of detailed portfolio information objects.

          
          

          - *(dict) --* 

            Detailed portfolio information.

            
            

            - **Id** *(string) --* 

              The identifier for the portfolio.

              
            

            - **ARN** *(string) --* 

              The ARN assigned to the portfolio.

              
            

            - **DisplayName** *(string) --* 

              The name to use for display purposes.

              
            

            - **Description** *(string) --* 

              The text description of the portfolio.

              
            

            - **CreatedTime** *(datetime) --* 

              The UTC timestamp of the creation time.

              
            

            - **ProviderName** *(string) --* 

              The name of the portfolio provider.

              
        
      
        

        - **NextPageToken** *(string) --* 

          The page token to use to retrieve the next page of results for this operation. If there are no more pages, this value is null.

          
    

  .. py:method:: list_constraints_for_portfolio(**kwargs)

    

    Retrieves detailed constraint information for the specified portfolio and product.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/ListConstraintsForPortfolio>`_    


    **Request Syntax** 
    ::

      response = client.list_constraints_for_portfolio(
          AcceptLanguage='string',
          PortfolioId='string',
          ProductId='string',
          PageSize=123,
          PageToken='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type PortfolioId: string
    :param PortfolioId: **[REQUIRED]** 

      The portfolio identifier.

      

    
    :type ProductId: string
    :param ProductId: 

      The product identifier.

      

    
    :type PageSize: integer
    :param PageSize: 

      The maximum number of items to return in the results. If more results exist than fit in the specified ``PageSize`` , the value of ``NextPageToken`` in the response is non-null.

      

    
    :type PageToken: string
    :param PageToken: 

      The page token of the first page retrieved. If null, this retrieves the first page of size ``PageSize`` .

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ConstraintDetails': [
                {
                    'ConstraintId': 'string',
                    'Type': 'string',
                    'Description': 'string',
                    'Owner': 'string'
                },
            ],
            'NextPageToken': 'string'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ConstraintDetails** *(list) --* 

          List of detailed constraint information objects.

          
          

          - *(dict) --* 

            Detailed constraint information.

            
            

            - **ConstraintId** *(string) --* 

              The identifier of the constraint.

              
            

            - **Type** *(string) --* 

              The type of the constraint.

              
            

            - **Description** *(string) --* 

              The text description of the constraint.

              
            

            - **Owner** *(string) --* 

              The owner of the constraint.

              
        
      
        

        - **NextPageToken** *(string) --* 

          The page token to use to retrieve the next page of results for this operation. If there are no more pages, this value is null.

          
    

  .. py:method:: list_launch_paths(**kwargs)

    

    Returns a paginated list of all paths to a specified product. A path is how the user has access to a specified product, and is necessary when provisioning a product. A path also determines the constraints put on the product.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/ListLaunchPaths>`_    


    **Request Syntax** 
    ::

      response = client.list_launch_paths(
          AcceptLanguage='string',
          ProductId='string',
          PageSize=123,
          PageToken='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type ProductId: string
    :param ProductId: **[REQUIRED]** 

      The product identifier. Identifies the product for which to retrieve ``LaunchPathSummaries`` information.

      

    
    :type PageSize: integer
    :param PageSize: 

      The maximum number of items to return in the results. If more results exist than fit in the specified ``PageSize`` , the value of ``NextPageToken`` in the response is non-null.

      

    
    :type PageToken: string
    :param PageToken: 

      The page token of the first page retrieved. If null, this retrieves the first page of size ``PageSize`` .

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'LaunchPathSummaries': [
                {
                    'Id': 'string',
                    'ConstraintSummaries': [
                        {
                            'Type': 'string',
                            'Description': 'string'
                        },
                    ],
                    'Tags': [
                        {
                            'Key': 'string',
                            'Value': 'string'
                        },
                    ],
                    'Name': 'string'
                },
            ],
            'NextPageToken': 'string'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **LaunchPathSummaries** *(list) --* 

          List of launch path information summaries for the specified ``PageToken`` .

          
          

          - *(dict) --* 

            Summary information about a path for a user to have access to a specified product.

            
            

            - **Id** *(string) --* 

              The unique identifier of the product path.

              
            

            - **ConstraintSummaries** *(list) --* 

              List of constraints on the portfolio-product relationship.

              
              

              - *(dict) --* 

                An administrator-specified constraint to apply when provisioning a product.

                
                

                - **Type** *(string) --* 

                  The type of the constraint. 

                  
                

                - **Description** *(string) --* 

                  The text description of the constraint.

                  
            
          
            

            - **Tags** *(list) --* 

              List of tags used by this launch path.

              
              

              - *(dict) --* 

                Key-value pairs to associate with this provisioning. These tags are entirely discretionary and are propagated to the resources created in the provisioning.

                
                

                - **Key** *(string) --* 

                  The ``ProvisioningArtifactParameter.TagKey`` parameter from  DescribeProvisioningParameters .

                  
                

                - **Value** *(string) --* 

                  The desired value for this key.

                  
            
          
            

            - **Name** *(string) --* 

              Corresponds to the name of the portfolio to which the user was assigned.

              
        
      
        

        - **NextPageToken** *(string) --* 

          The page token to use to retrieve the next page of results for this operation. If there are no more pages, this value is null.

          
    

  .. py:method:: list_portfolio_access(**kwargs)

    

    Lists the account IDs that have been authorized sharing of the specified portfolio.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/ListPortfolioAccess>`_    


    **Request Syntax** 
    ::

      response = client.list_portfolio_access(
          AcceptLanguage='string',
          PortfolioId='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type PortfolioId: string
    :param PortfolioId: **[REQUIRED]** 

      The portfolio identifier.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'AccountIds': [
                'string',
            ],
            'NextPageToken': 'string'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **AccountIds** *(list) --* 

          List of account IDs associated with access to the portfolio.

          
          

          - *(string) --* 
      
        

        - **NextPageToken** *(string) --* 

          The page token to use to retrieve the next page of results for this operation. If there are no more pages, this value is null.

          
    

  .. py:method:: list_portfolios(**kwargs)

    

    Lists all portfolios in the catalog.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/ListPortfolios>`_    


    **Request Syntax** 
    ::

      response = client.list_portfolios(
          AcceptLanguage='string',
          PageToken='string',
          PageSize=123
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type PageToken: string
    :param PageToken: 

      The page token of the first page retrieved. If null, this retrieves the first page of size ``PageSize`` .

      

    
    :type PageSize: integer
    :param PageSize: 

      The maximum number of items to return in the results. If more results exist than fit in the specified ``PageSize`` , the value of ``NextPageToken`` in the response is non-null.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'PortfolioDetails': [
                {
                    'Id': 'string',
                    'ARN': 'string',
                    'DisplayName': 'string',
                    'Description': 'string',
                    'CreatedTime': datetime(2015, 1, 1),
                    'ProviderName': 'string'
                },
            ],
            'NextPageToken': 'string'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **PortfolioDetails** *(list) --* 

          List of detailed portfolio information objects.

          
          

          - *(dict) --* 

            Detailed portfolio information.

            
            

            - **Id** *(string) --* 

              The identifier for the portfolio.

              
            

            - **ARN** *(string) --* 

              The ARN assigned to the portfolio.

              
            

            - **DisplayName** *(string) --* 

              The name to use for display purposes.

              
            

            - **Description** *(string) --* 

              The text description of the portfolio.

              
            

            - **CreatedTime** *(datetime) --* 

              The UTC timestamp of the creation time.

              
            

            - **ProviderName** *(string) --* 

              The name of the portfolio provider.

              
        
      
        

        - **NextPageToken** *(string) --* 

          The page token to use to retrieve the next page of results for this operation. If there are no more pages, this value is null.

          
    

  .. py:method:: list_portfolios_for_product(**kwargs)

    

    Lists all portfolios that the specified product is associated with.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/ListPortfoliosForProduct>`_    


    **Request Syntax** 
    ::

      response = client.list_portfolios_for_product(
          AcceptLanguage='string',
          ProductId='string',
          PageToken='string',
          PageSize=123
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type ProductId: string
    :param ProductId: **[REQUIRED]** 

      The product identifier.

      

    
    :type PageToken: string
    :param PageToken: 

      The page token of the first page retrieved. If null, this retrieves the first page of size ``PageSize`` .

      

    
    :type PageSize: integer
    :param PageSize: 

      The maximum number of items to return in the results. If more results exist than fit in the specified ``PageSize`` , the value of ``NextPageToken`` in the response is non-null.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'PortfolioDetails': [
                {
                    'Id': 'string',
                    'ARN': 'string',
                    'DisplayName': 'string',
                    'Description': 'string',
                    'CreatedTime': datetime(2015, 1, 1),
                    'ProviderName': 'string'
                },
            ],
            'NextPageToken': 'string'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **PortfolioDetails** *(list) --* 

          List of detailed portfolio information objects.

          
          

          - *(dict) --* 

            Detailed portfolio information.

            
            

            - **Id** *(string) --* 

              The identifier for the portfolio.

              
            

            - **ARN** *(string) --* 

              The ARN assigned to the portfolio.

              
            

            - **DisplayName** *(string) --* 

              The name to use for display purposes.

              
            

            - **Description** *(string) --* 

              The text description of the portfolio.

              
            

            - **CreatedTime** *(datetime) --* 

              The UTC timestamp of the creation time.

              
            

            - **ProviderName** *(string) --* 

              The name of the portfolio provider.

              
        
      
        

        - **NextPageToken** *(string) --* 

          The page token to use to retrieve the next page of results for this operation. If there are no more pages, this value is null.

          
    

  .. py:method:: list_principals_for_portfolio(**kwargs)

    

    Lists all principal ARNs associated with the specified portfolio.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/ListPrincipalsForPortfolio>`_    


    **Request Syntax** 
    ::

      response = client.list_principals_for_portfolio(
          AcceptLanguage='string',
          PortfolioId='string',
          PageSize=123,
          PageToken='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type PortfolioId: string
    :param PortfolioId: **[REQUIRED]** 

      The portfolio identifier.

      

    
    :type PageSize: integer
    :param PageSize: 

      The maximum number of items to return in the results. If more results exist than fit in the specified ``PageSize`` , the value of ``NextPageToken`` in the response is non-null.

      

    
    :type PageToken: string
    :param PageToken: 

      The page token of the first page retrieved. If null, this retrieves the first page of size ``PageSize`` .

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'Principals': [
                {
                    'PrincipalARN': 'string',
                    'PrincipalType': 'IAM'
                },
            ],
            'NextPageToken': 'string'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **Principals** *(list) --* 

          The IAM principals (users or roles) associated with the portfolio.

          
          

          - *(dict) --* 

            A principal's ARN and type.

            
            

            - **PrincipalARN** *(string) --* 

              The ARN representing the principal (IAM user, role, or group).

              
            

            - **PrincipalType** *(string) --* 

              The principal type. Must be ``IAM``  

              
        
      
        

        - **NextPageToken** *(string) --* 

          The page token to use to retrieve the next page of results for this operation. If there are no more pages, this value is null.

          
    

  .. py:method:: list_provisioning_artifacts(**kwargs)

    

    Lists all provisioning artifacts associated with the specified product.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/ListProvisioningArtifacts>`_    


    **Request Syntax** 
    ::

      response = client.list_provisioning_artifacts(
          AcceptLanguage='string',
          ProductId='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type ProductId: string
    :param ProductId: **[REQUIRED]** 

      The product identifier.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ProvisioningArtifactDetails': [
                {
                    'Id': 'string',
                    'Name': 'string',
                    'Description': 'string',
                    'Type': 'CLOUD_FORMATION_TEMPLATE'|'MARKETPLACE_AMI'|'MARKETPLACE_CAR',
                    'CreatedTime': datetime(2015, 1, 1)
                },
            ],
            'NextPageToken': 'string'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ProvisioningArtifactDetails** *(list) --* 

          List of detailed provisioning artifact information objects.

          
          

          - *(dict) --* 

            Detailed provisioning artifact information.

            
            

            - **Id** *(string) --* 

              The identifier of the provisioning artifact. This is sometimes referred to as the product version.

              
            

            - **Name** *(string) --* 

              The name assigned to the provisioning artifact.

              
            

            - **Description** *(string) --* 

              The text description of the provisioning artifact.

              
            

            - **Type** *(string) --* 

              The type of the provisioning artifact. The following provisioning artifact types are used by AWS Marketplace products:

               

               ``MARKETPLACE_AMI`` - AMI products.

               

               ``MARKETPLACE_CAR`` - CAR (Cluster and AWS Resources) products.

              
            

            - **CreatedTime** *(datetime) --* 

              The UTC timestamp of the creation time.

              
        
      
        

        - **NextPageToken** *(string) --* 

          The page token to use to retrieve the next page of results for this operation. If there are no more pages, this value is null.

          
    

  .. py:method:: list_record_history(**kwargs)

    

    Returns a paginated list of all performed requests, in the form of RecordDetails objects that are filtered as specified.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/ListRecordHistory>`_    


    **Request Syntax** 
    ::

      response = client.list_record_history(
          AcceptLanguage='string',
          AccessLevelFilter={
              'Key': 'Account'|'Role'|'User',
              'Value': 'string'
          },
          SearchFilter={
              'Key': 'string',
              'Value': 'string'
          },
          PageSize=123,
          PageToken='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type AccessLevelFilter: dict
    :param AccessLevelFilter: 

      The access level for obtaining results. If left unspecified, ``User`` level access is used.

      

    
      - **Key** *(string) --* 

        Specifies the access level.

         

         ``Account`` allows results at the account level. 

         

         ``Role`` allows results based on the federated role of the specified user.

         

         ``User`` allows results limited to the specified user. 

        

      
      - **Value** *(string) --* 

        Specifies the user to which the access level applies. A value of ``Self`` is currently supported.

        

      
    
    :type SearchFilter: dict
    :param SearchFilter: 

      The filter to limit search results. 

      

    
      - **Key** *(string) --* 

        The filter key.

        

      
      - **Value** *(string) --* 

        The filter value for ``Key`` .

        

      
    
    :type PageSize: integer
    :param PageSize: 

      The maximum number of items to return in the results. If more results exist than fit in the specified ``PageSize`` , the value of ``NextPageToken`` in the response is non-null.

      

    
    :type PageToken: string
    :param PageToken: 

      The page token of the first page retrieved. If null, this retrieves the first page of size ``PageSize`` .

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'RecordDetails': [
                {
                    'RecordId': 'string',
                    'ProvisionedProductName': 'string',
                    'Status': 'CREATED'|'IN_PROGRESS'|'IN_PROGRESS_IN_ERROR'|'SUCCEEDED'|'FAILED',
                    'CreatedTime': datetime(2015, 1, 1),
                    'UpdatedTime': datetime(2015, 1, 1),
                    'ProvisionedProductType': 'string',
                    'RecordType': 'string',
                    'ProvisionedProductId': 'string',
                    'ProductId': 'string',
                    'ProvisioningArtifactId': 'string',
                    'PathId': 'string',
                    'RecordErrors': [
                        {
                            'Code': 'string',
                            'Description': 'string'
                        },
                    ],
                    'RecordTags': [
                        {
                            'Key': 'string',
                            'Value': 'string'
                        },
                    ]
                },
            ],
            'NextPageToken': 'string'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **RecordDetails** *(list) --* 

          A list of record detail objects, listed in reverse chronological order.

          
          

          - *(dict) --* 

            The full details of a specific ProvisionedProduct object.

            
            

            - **RecordId** *(string) --* 

              The identifier of the ProvisionedProduct object record.

              
            

            - **ProvisionedProductName** *(string) --* 

              The user-friendly name of the ProvisionedProduct object.

              
            

            - **Status** *(string) --* 

              The status of the ProvisionedProduct object.

               

               ``CREATED`` - Request created but the operation has not yet started.

               

               ``IN_PROGRESS`` - The requested operation is in-progress.

               

               ``IN_PROGRESS_IN_ERROR`` - The provisioned product is under change but the requested operation failed and some remediation is occurring. For example, a rollback.

               

               ``SUCCEEDED`` - The requested operation has successfully completed.

               

               ``FAILED`` - The requested operation has completed but has failed. Investigate using the error messages returned.

              
            

            - **CreatedTime** *(datetime) --* 

              The UTC timestamp of the creation time.

              
            

            - **UpdatedTime** *(datetime) --* 

              The time when the record for the ProvisionedProduct object was last updated.

              
            

            - **ProvisionedProductType** *(string) --* 

              The type of the ProvisionedProduct object.

              
            

            - **RecordType** *(string) --* 

              The record type for this record.

              
            

            - **ProvisionedProductId** *(string) --* 

              The identifier of the ProvisionedProduct object.

              
            

            - **ProductId** *(string) --* 

              The product identifier.

              
            

            - **ProvisioningArtifactId** *(string) --* 

              The provisioning artifact identifier for this product. This is sometimes referred to as the product version.

              
            

            - **PathId** *(string) --* 

              The identifier of the path for this product's provisioning.

              
            

            - **RecordErrors** *(list) --* 

              A list of errors that occurred while processing the request.

              
              

              - *(dict) --* 

                The error code and description resulting from an operation.

                
                

                - **Code** *(string) --* 

                  The numeric value of the error.

                  
                

                - **Description** *(string) --* 

                  The text description of the error.

                  
            
          
            

            - **RecordTags** *(list) --* 

              List of tags associated with this record.

              
              

              - *(dict) --* 

                A tag associated with the record, stored as a key-value pair.

                
                

                - **Key** *(string) --* 

                  The key for this tag.

                  
                

                - **Value** *(string) --* 

                  The value for this tag.

                  
            
          
        
      
        

        - **NextPageToken** *(string) --* 

          The page token to use to retrieve the next page of results for this operation. If there are no more pages, this value is null.

          
    

  .. py:method:: list_resources_for_tag_option(**kwargs)

    

    Lists resources associated with a TagOption.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/ListResourcesForTagOption>`_    


    **Request Syntax** 
    ::

      response = client.list_resources_for_tag_option(
          TagOptionId='string',
          ResourceType='string',
          PageSize=123,
          PageToken='string'
      )
    :type TagOptionId: string
    :param TagOptionId: **[REQUIRED]** 

      Identifier of the TagOption.

      

    
    :type ResourceType: string
    :param ResourceType: 

      Resource type.

      

    
    :type PageSize: integer
    :param PageSize: 

      The maximum number of items to return in the results. If more results exist than fit in the specified ``PageSize`` , the value of ``NextPageToken`` in the response is non-null.

      

    
    :type PageToken: string
    :param PageToken: 

      The page token of the first page retrieved. If null, this retrieves the first page of size ``PageSize`` .

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ResourceDetails': [
                {
                    'Id': 'string',
                    'ARN': 'string',
                    'Name': 'string',
                    'Description': 'string',
                    'CreatedTime': datetime(2015, 1, 1)
                },
            ],
            'PageToken': 'string'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ResourceDetails** *(list) --* 

          The resulting detailed resource information.

          
          

          - *(dict) --* 

            Detailed resource information.

            
            

            - **Id** *(string) --* 

              Identifier of the resource.

              
            

            - **ARN** *(string) --* 

              ARN of the resource.

              
            

            - **Name** *(string) --* 

              Name of the resource.

              
            

            - **Description** *(string) --* 

              Description of the resource.

              
            

            - **CreatedTime** *(datetime) --* 

              Creation time of the resource.

              
        
      
        

        - **PageToken** *(string) --* 

          The page token of the first page retrieved. If null, this retrieves the first page of size ``PageSize`` .

          
    

  .. py:method:: list_tag_options(**kwargs)

    

    Lists detailed TagOptions information.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/ListTagOptions>`_    


    **Request Syntax** 
    ::

      response = client.list_tag_options(
          Filters={
              'Key': 'string',
              'Value': 'string',
              'Active': True|False
          },
          PageSize=123,
          PageToken='string'
      )
    :type Filters: dict
    :param Filters: 

      The list of filters with which to limit search results. If no search filters are specified, the output is all TagOptions. 

      

    
      - **Key** *(string) --* 

        The ListTagOptionsFilters key.

        

      
      - **Value** *(string) --* 

        The ListTagOptionsFilters value.

        

      
      - **Active** *(boolean) --* 

        The ListTagOptionsFilters active state.

        

      
    
    :type PageSize: integer
    :param PageSize: 

      The maximum number of items to return in the results. If more results exist than fit in the specified ``PageSize`` , the value of ``NextPageToken`` in the response is non-null.

      

    
    :type PageToken: string
    :param PageToken: 

      The page token of the first page retrieved. If null, this retrieves the first page of size ``PageSize`` .

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'TagOptionDetails': [
                {
                    'Key': 'string',
                    'Value': 'string',
                    'Active': True|False,
                    'Id': 'string'
                },
            ],
            'PageToken': 'string'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **TagOptionDetails** *(list) --* 

          The resulting detailed TagOption information.

          
          

          - *(dict) --* 

            The TagOption details.

            
            

            - **Key** *(string) --* 

              The TagOptionDetail key.

              
            

            - **Value** *(string) --* 

              The TagOptionDetail value.

              
            

            - **Active** *(boolean) --* 

              The TagOptionDetail active state.

              
            

            - **Id** *(string) --* 

              The TagOptionDetail identifier.

              
        
      
        

        - **PageToken** *(string) --* 

          The page token of the first page retrieved. If null, this retrieves the first page of size ``PageSize`` .

          
    

  .. py:method:: provision_product(**kwargs)

    

    Requests a *provision* of a specified product. A *provisioned product* is a resourced instance for a product. For example, provisioning a CloudFormation-template-backed product results in launching a CloudFormation stack and all the underlying resources that come with it. 

     

    You can check the status of this request using the  DescribeRecord operation. The error "Parameter validation failed: Missing required parameter in Tags[*N* ]:*Value* " indicates that your request contains a tag which has a tag key but no corresponding tag value (value is empty or null). Your call may have included values returned from a ``DescribeProvisioningParameters`` call that resulted in a TagOption key with an empty list. This happens when TagOption keys are in conflict. For more information, see  DescribeProvisioningParameters .

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/ProvisionProduct>`_    


    **Request Syntax** 
    ::

      response = client.provision_product(
          AcceptLanguage='string',
          ProductId='string',
          ProvisioningArtifactId='string',
          PathId='string',
          ProvisionedProductName='string',
          ProvisioningParameters=[
              {
                  'Key': 'string',
                  'Value': 'string'
              },
          ],
          Tags=[
              {
                  'Key': 'string',
                  'Value': 'string'
              },
          ],
          NotificationArns=[
              'string',
          ],
          ProvisionToken='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type ProductId: string
    :param ProductId: **[REQUIRED]** 

      The product identifier.

      

    
    :type ProvisioningArtifactId: string
    :param ProvisioningArtifactId: **[REQUIRED]** 

      The provisioning artifact identifier for this product. This is sometimes referred to as the product version.

      

    
    :type PathId: string
    :param PathId: 

      The identifier of the path for this product's provisioning. This value is optional if the product has a default path, and is required if there is more than one path for the specified product.

      

    
    :type ProvisionedProductName: string
    :param ProvisionedProductName: **[REQUIRED]** 

      A user-friendly name to identify the ProvisionedProduct object. This value must be unique for the AWS account and cannot be updated after the product is provisioned.

      

    
    :type ProvisioningParameters: list
    :param ProvisioningParameters: 

      Parameters specified by the administrator that are required for provisioning the product.

      

    
      - *(dict) --* 

        The parameter key-value pairs used to provision a product.

        

      
        - **Key** *(string) --* 

          The ``ProvisioningArtifactParameter.ParameterKey`` parameter from  DescribeProvisioningParameters .

          

        
        - **Value** *(string) --* 

          The value to use for provisioning. Any constraints on this value can be found in ``ProvisioningArtifactParameter`` for ``Key`` .

          

        
      
  
    :type Tags: list
    :param Tags: 

      A list of tags to use as provisioning options.

      

    
      - *(dict) --* 

        Key-value pairs to associate with this provisioning. These tags are entirely discretionary and are propagated to the resources created in the provisioning.

        

      
        - **Key** *(string) --* **[REQUIRED]** 

          The ``ProvisioningArtifactParameter.TagKey`` parameter from  DescribeProvisioningParameters .

          

        
        - **Value** *(string) --* **[REQUIRED]** 

          The desired value for this key.

          

        
      
  
    :type NotificationArns: list
    :param NotificationArns: 

      Passed to CloudFormation. The SNS topic ARNs to which to publish stack-related events.

      

    
      - *(string) --* 

      
  
    :type ProvisionToken: string
    :param ProvisionToken: **[REQUIRED]** 

      An idempotency token that uniquely identifies the provisioning request. 

      This field is autopopulated if not provided.

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'RecordDetail': {
                'RecordId': 'string',
                'ProvisionedProductName': 'string',
                'Status': 'CREATED'|'IN_PROGRESS'|'IN_PROGRESS_IN_ERROR'|'SUCCEEDED'|'FAILED',
                'CreatedTime': datetime(2015, 1, 1),
                'UpdatedTime': datetime(2015, 1, 1),
                'ProvisionedProductType': 'string',
                'RecordType': 'string',
                'ProvisionedProductId': 'string',
                'ProductId': 'string',
                'ProvisioningArtifactId': 'string',
                'PathId': 'string',
                'RecordErrors': [
                    {
                        'Code': 'string',
                        'Description': 'string'
                    },
                ],
                'RecordTags': [
                    {
                        'Key': 'string',
                        'Value': 'string'
                    },
                ]
            }
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **RecordDetail** *(dict) --* 

          The detailed result of the  ProvisionProduct request, containing the inputs made to that request, the current state of the request, a pointer to the ProvisionedProduct object of the request, and a list of any errors that the request encountered. 

          
          

          - **RecordId** *(string) --* 

            The identifier of the ProvisionedProduct object record.

            
          

          - **ProvisionedProductName** *(string) --* 

            The user-friendly name of the ProvisionedProduct object.

            
          

          - **Status** *(string) --* 

            The status of the ProvisionedProduct object.

             

             ``CREATED`` - Request created but the operation has not yet started.

             

             ``IN_PROGRESS`` - The requested operation is in-progress.

             

             ``IN_PROGRESS_IN_ERROR`` - The provisioned product is under change but the requested operation failed and some remediation is occurring. For example, a rollback.

             

             ``SUCCEEDED`` - The requested operation has successfully completed.

             

             ``FAILED`` - The requested operation has completed but has failed. Investigate using the error messages returned.

            
          

          - **CreatedTime** *(datetime) --* 

            The UTC timestamp of the creation time.

            
          

          - **UpdatedTime** *(datetime) --* 

            The time when the record for the ProvisionedProduct object was last updated.

            
          

          - **ProvisionedProductType** *(string) --* 

            The type of the ProvisionedProduct object.

            
          

          - **RecordType** *(string) --* 

            The record type for this record.

            
          

          - **ProvisionedProductId** *(string) --* 

            The identifier of the ProvisionedProduct object.

            
          

          - **ProductId** *(string) --* 

            The product identifier.

            
          

          - **ProvisioningArtifactId** *(string) --* 

            The provisioning artifact identifier for this product. This is sometimes referred to as the product version.

            
          

          - **PathId** *(string) --* 

            The identifier of the path for this product's provisioning.

            
          

          - **RecordErrors** *(list) --* 

            A list of errors that occurred while processing the request.

            
            

            - *(dict) --* 

              The error code and description resulting from an operation.

              
              

              - **Code** *(string) --* 

                The numeric value of the error.

                
              

              - **Description** *(string) --* 

                The text description of the error.

                
          
        
          

          - **RecordTags** *(list) --* 

            List of tags associated with this record.

            
            

            - *(dict) --* 

              A tag associated with the record, stored as a key-value pair.

              
              

              - **Key** *(string) --* 

                The key for this tag.

                
              

              - **Value** *(string) --* 

                The value for this tag.

                
          
        
      
    

  .. py:method:: reject_portfolio_share(**kwargs)

    

    Rejects an offer to share a portfolio.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/RejectPortfolioShare>`_    


    **Request Syntax** 
    ::

      response = client.reject_portfolio_share(
          AcceptLanguage='string',
          PortfolioId='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type PortfolioId: string
    :param PortfolioId: **[REQUIRED]** 

      The portfolio identifier.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {}
        
      **Response Structure** 

      

      - *(dict) --* 
    

  .. py:method:: scan_provisioned_products(**kwargs)

    

    Returns a paginated list of all the ProvisionedProduct objects that are currently available (not terminated). 

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/ScanProvisionedProducts>`_    


    **Request Syntax** 
    ::

      response = client.scan_provisioned_products(
          AcceptLanguage='string',
          AccessLevelFilter={
              'Key': 'Account'|'Role'|'User',
              'Value': 'string'
          },
          PageSize=123,
          PageToken='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type AccessLevelFilter: dict
    :param AccessLevelFilter: 

      The access level for obtaining results. If left unspecified, ``User`` level access is used.

      

    
      - **Key** *(string) --* 

        Specifies the access level.

         

         ``Account`` allows results at the account level. 

         

         ``Role`` allows results based on the federated role of the specified user.

         

         ``User`` allows results limited to the specified user. 

        

      
      - **Value** *(string) --* 

        Specifies the user to which the access level applies. A value of ``Self`` is currently supported.

        

      
    
    :type PageSize: integer
    :param PageSize: 

      The maximum number of items to return in the results. If more results exist than fit in the specified ``PageSize`` , the value of ``NextPageToken`` in the response is non-null.

      

    
    :type PageToken: string
    :param PageToken: 

      The page token of the first page retrieved. If null, this retrieves the first page of size ``PageSize`` .

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ProvisionedProducts': [
                {
                    'Name': 'string',
                    'Arn': 'string',
                    'Type': 'string',
                    'Id': 'string',
                    'Status': 'AVAILABLE'|'UNDER_CHANGE'|'TAINTED'|'ERROR',
                    'StatusMessage': 'string',
                    'CreatedTime': datetime(2015, 1, 1),
                    'IdempotencyToken': 'string',
                    'LastRecordId': 'string'
                },
            ],
            'NextPageToken': 'string'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ProvisionedProducts** *(list) --* 

          A list of ProvisionedProduct detail objects.

          
          

          - *(dict) --* 

            Detailed information about a ProvisionedProduct object.

            
            

            - **Name** *(string) --* 

              The user-friendly name of the ProvisionedProduct object.

              
            

            - **Arn** *(string) --* 

              The ARN associated with the ProvisionedProduct object.

              
            

            - **Type** *(string) --* 

              The type of the ProvisionedProduct object.

              
            

            - **Id** *(string) --* 

              The identifier of the ProvisionedProduct object.

              
            

            - **Status** *(string) --* 

              The current status of the ProvisionedProduct.

               

               ``AVAILABLE`` - Stable state, ready to perform any operation. The most recent action request succeeded and completed.

               

               ``UNDER_CHANGE`` - Transitive state, operations performed may or may not have valid results. Wait for an ``AVAILABLE`` status before performing operations.

               

               ``TAINTED`` - Stable state, ready to perform any operation. The stack has completed the requested operation but is not exactly what was requested. For example, a request to update to a new version failed and the stack rolled back to the current version. 

               

               ``ERROR`` - Something unexpected happened such that the provisioned product exists but the stack is not running. For example, CloudFormation received an invalid parameter value and could not launch the stack.

              
            

            - **StatusMessage** *(string) --* 

              The current status message of the ProvisionedProduct.

              
            

            - **CreatedTime** *(datetime) --* 

              The UTC timestamp of the creation time.

              
            

            - **IdempotencyToken** *(string) --* 

              A token to disambiguate duplicate requests. You can use the same input in multiple requests, provided that you also specify a different idempotency token for each request.

              
            

            - **LastRecordId** *(string) --* 

              The record identifier of the last request performed on this ProvisionedProduct object.

              
        
      
        

        - **NextPageToken** *(string) --* 

          The page token to use to retrieve the next page of results for this operation. If there are no more pages, this value is null.

          
    

  .. py:method:: search_products(**kwargs)

    

    Returns a paginated list all of the ``Products`` objects to which the caller has access. 

     

    The output of this operation can be used as input for other operations, such as  DescribeProductView .

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/SearchProducts>`_    


    **Request Syntax** 
    ::

      response = client.search_products(
          AcceptLanguage='string',
          Filters={
              'string': [
                  'string',
              ]
          },
          PageSize=123,
          SortBy='Title'|'VersionCount'|'CreationDate',
          SortOrder='ASCENDING'|'DESCENDING',
          PageToken='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type Filters: dict
    :param Filters: 

      The list of filters with which to limit search results. If no search filters are specified, the output is all the products to which the calling user has access. 

      

    
      - *(string) --* 

      
        - *(list) --* 

        
          - *(string) --* 

          
      
  

    :type PageSize: integer
    :param PageSize: 

      The maximum number of items to return in the results. If more results exist than fit in the specified ``PageSize`` , the value of ``NextPageToken`` in the response is non-null.

      

    
    :type SortBy: string
    :param SortBy: 

      The sort field specifier. If no value is specified, results are not sorted.

      

    
    :type SortOrder: string
    :param SortOrder: 

      The sort order specifier. If no value is specified, results are not sorted.

      

    
    :type PageToken: string
    :param PageToken: 

      The page token of the first page retrieved. If null, this retrieves the first page of size ``PageSize`` .

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ProductViewSummaries': [
                {
                    'Id': 'string',
                    'ProductId': 'string',
                    'Name': 'string',
                    'Owner': 'string',
                    'ShortDescription': 'string',
                    'Type': 'CLOUD_FORMATION_TEMPLATE'|'MARKETPLACE',
                    'Distributor': 'string',
                    'HasDefaultPath': True|False,
                    'SupportEmail': 'string',
                    'SupportDescription': 'string',
                    'SupportUrl': 'string'
                },
            ],
            'ProductViewAggregations': {
                'string': [
                    {
                        'Value': 'string',
                        'ApproximateCount': 123
                    },
                ]
            },
            'NextPageToken': 'string'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ProductViewSummaries** *(list) --* 

          A list of the product view summary objects.

          
          

          - *(dict) --* 

            The summary metadata about the specified product.

            
            

            - **Id** *(string) --* 

              The product view identifier.

              
            

            - **ProductId** *(string) --* 

              The product identifier.

              
            

            - **Name** *(string) --* 

              The name of the product.

              
            

            - **Owner** *(string) --* 

              The owner of the product. Contact the product administrator for the significance of this value.

              
            

            - **ShortDescription** *(string) --* 

              Short description of the product.

              
            

            - **Type** *(string) --* 

              The product type. Contact the product administrator for the significance of this value. If this value is ``MARKETPLACE`` , the product was created by AWS Marketplace.

              
            

            - **Distributor** *(string) --* 

              The distributor of the product. Contact the product administrator for the significance of this value.

              
            

            - **HasDefaultPath** *(boolean) --* 

              A value of ``false`` indicates that the product does not have a default path, while a value of ``true`` indicates that it does. If it's false, call  ListLaunchPaths to disambiguate between paths. If true,  ListLaunchPaths is not required, and the output of the  ProductViewSummary operation can be used directly with  DescribeProvisioningParameters .

              
            

            - **SupportEmail** *(string) --* 

              The email contact information to obtain support for this Product.

              
            

            - **SupportDescription** *(string) --* 

              The description of the support for this Product.

              
            

            - **SupportUrl** *(string) --* 

              The URL information to obtain support for this Product.

              
        
      
        

        - **ProductViewAggregations** *(dict) --* 

          A list of the product view aggregation value objects.

          
          

          - *(string) --* 
            

            - *(list) --* 
              

              - *(dict) --* 

                A single product view aggregation value/count pair, containing metadata about each product to which the calling user has access.

                
                

                - **Value** *(string) --* 

                  The value of the product view aggregation.

                  
                

                - **ApproximateCount** *(integer) --* 

                  An approximate count of the products that match the value.

                  
            
          
      
    
        

        - **NextPageToken** *(string) --* 

          The page token to use to retrieve the next page of results for this operation. If there are no more pages, this value is null.

          
    

  .. py:method:: search_products_as_admin(**kwargs)

    

    Retrieves summary and status information about all products created within the caller's account. If a portfolio ID is provided, this operation retrieves information for only those products that are associated with the specified portfolio.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/SearchProductsAsAdmin>`_    


    **Request Syntax** 
    ::

      response = client.search_products_as_admin(
          AcceptLanguage='string',
          PortfolioId='string',
          Filters={
              'string': [
                  'string',
              ]
          },
          SortBy='Title'|'VersionCount'|'CreationDate',
          SortOrder='ASCENDING'|'DESCENDING',
          PageToken='string',
          PageSize=123,
          ProductSource='ACCOUNT'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type PortfolioId: string
    :param PortfolioId: 

      The portfolio identifier.

      

    
    :type Filters: dict
    :param Filters: 

      The list of filters with which to limit search results. If no search filters are specified, the output is all the products to which the administrator has access.

      

    
      - *(string) --* 

      
        - *(list) --* 

        
          - *(string) --* 

          
      
  

    :type SortBy: string
    :param SortBy: 

      The sort field specifier. If no value is specified, results are not sorted.

      

    
    :type SortOrder: string
    :param SortOrder: 

      The sort order specifier. If no value is specified, results are not sorted.

      

    
    :type PageToken: string
    :param PageToken: 

      The page token of the first page retrieved. If null, this retrieves the first page of size ``PageSize`` .

      

    
    :type PageSize: integer
    :param PageSize: 

      The maximum number of items to return in the results. If more results exist than fit in the specified ``PageSize`` , the value of ``NextPageToken`` in the response is non-null.

      

    
    :type ProductSource: string
    :param ProductSource: 

      Access level of the source of the product.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ProductViewDetails': [
                {
                    'ProductViewSummary': {
                        'Id': 'string',
                        'ProductId': 'string',
                        'Name': 'string',
                        'Owner': 'string',
                        'ShortDescription': 'string',
                        'Type': 'CLOUD_FORMATION_TEMPLATE'|'MARKETPLACE',
                        'Distributor': 'string',
                        'HasDefaultPath': True|False,
                        'SupportEmail': 'string',
                        'SupportDescription': 'string',
                        'SupportUrl': 'string'
                    },
                    'Status': 'AVAILABLE'|'CREATING'|'FAILED',
                    'ProductARN': 'string',
                    'CreatedTime': datetime(2015, 1, 1)
                },
            ],
            'NextPageToken': 'string'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ProductViewDetails** *(list) --* 

          List of detailed product view information objects.

          
          

          - *(dict) --* 

            Detailed product view information.

            
            

            - **ProductViewSummary** *(dict) --* 

              The summary metadata about the specified product view.

              
              

              - **Id** *(string) --* 

                The product view identifier.

                
              

              - **ProductId** *(string) --* 

                The product identifier.

                
              

              - **Name** *(string) --* 

                The name of the product.

                
              

              - **Owner** *(string) --* 

                The owner of the product. Contact the product administrator for the significance of this value.

                
              

              - **ShortDescription** *(string) --* 

                Short description of the product.

                
              

              - **Type** *(string) --* 

                The product type. Contact the product administrator for the significance of this value. If this value is ``MARKETPLACE`` , the product was created by AWS Marketplace.

                
              

              - **Distributor** *(string) --* 

                The distributor of the product. Contact the product administrator for the significance of this value.

                
              

              - **HasDefaultPath** *(boolean) --* 

                A value of ``false`` indicates that the product does not have a default path, while a value of ``true`` indicates that it does. If it's false, call  ListLaunchPaths to disambiguate between paths. If true,  ListLaunchPaths is not required, and the output of the  ProductViewSummary operation can be used directly with  DescribeProvisioningParameters .

                
              

              - **SupportEmail** *(string) --* 

                The email contact information to obtain support for this Product.

                
              

              - **SupportDescription** *(string) --* 

                The description of the support for this Product.

                
              

              - **SupportUrl** *(string) --* 

                The URL information to obtain support for this Product.

                
          
            

            - **Status** *(string) --* 

              Current status of the product.

               

               ``AVAILABLE`` - Product is available for use.

               

               ``CREATING`` - Creation of product started, not ready for use.

               

               ``FAILED`` - Action on product failed.

              
            

            - **ProductARN** *(string) --* 

              The ARN associated with the product.

              
            

            - **CreatedTime** *(datetime) --* 

              The UTC timestamp of the creation time.

              
        
      
        

        - **NextPageToken** *(string) --* 

          The page token to use to retrieve the next page of results for this operation. If there are no more pages, this value is null.

          
    

  .. py:method:: terminate_provisioned_product(**kwargs)

    

    Requests termination of an existing ProvisionedProduct object. If there are ``Tags`` associated with the object, they are terminated when the ProvisionedProduct object is terminated. 

     

    This operation does not delete any records associated with the ProvisionedProduct object.

     

    You can check the status of this request using the  DescribeRecord operation.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/TerminateProvisionedProduct>`_    


    **Request Syntax** 
    ::

      response = client.terminate_provisioned_product(
          ProvisionedProductName='string',
          ProvisionedProductId='string',
          TerminateToken='string',
          IgnoreErrors=True|False,
          AcceptLanguage='string'
      )
    :type ProvisionedProductName: string
    :param ProvisionedProductName: 

      The name of the ProvisionedProduct object to terminate. Specify either ``ProvisionedProductName`` or ``ProvisionedProductId`` , but not both.

      

    
    :type ProvisionedProductId: string
    :param ProvisionedProductId: 

      The identifier of the ProvisionedProduct object to terminate. Specify either ``ProvisionedProductName`` or ``ProvisionedProductId`` , but not both.

      

    
    :type TerminateToken: string
    :param TerminateToken: **[REQUIRED]** 

      An idempotency token that uniquely identifies the termination request. This token is only valid during the termination process. After the ProvisionedProduct object is terminated, further requests to terminate the same ProvisionedProduct object always return **ResourceNotFound** regardless of the value of ``TerminateToken`` .

      This field is autopopulated if not provided.

    
    :type IgnoreErrors: boolean
    :param IgnoreErrors: 

      If set to true, AWS Service Catalog stops managing the specified ProvisionedProduct object even if it cannot delete the underlying resources.

      

    
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'RecordDetail': {
                'RecordId': 'string',
                'ProvisionedProductName': 'string',
                'Status': 'CREATED'|'IN_PROGRESS'|'IN_PROGRESS_IN_ERROR'|'SUCCEEDED'|'FAILED',
                'CreatedTime': datetime(2015, 1, 1),
                'UpdatedTime': datetime(2015, 1, 1),
                'ProvisionedProductType': 'string',
                'RecordType': 'string',
                'ProvisionedProductId': 'string',
                'ProductId': 'string',
                'ProvisioningArtifactId': 'string',
                'PathId': 'string',
                'RecordErrors': [
                    {
                        'Code': 'string',
                        'Description': 'string'
                    },
                ],
                'RecordTags': [
                    {
                        'Key': 'string',
                        'Value': 'string'
                    },
                ]
            }
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **RecordDetail** *(dict) --* 

          The detailed result of the  TerminateProvisionedProduct request, containing the inputs made to that request, the current state of the request, a pointer to the ProvisionedProduct object that the request is modifying, and a list of any errors that the request encountered.

          
          

          - **RecordId** *(string) --* 

            The identifier of the ProvisionedProduct object record.

            
          

          - **ProvisionedProductName** *(string) --* 

            The user-friendly name of the ProvisionedProduct object.

            
          

          - **Status** *(string) --* 

            The status of the ProvisionedProduct object.

             

             ``CREATED`` - Request created but the operation has not yet started.

             

             ``IN_PROGRESS`` - The requested operation is in-progress.

             

             ``IN_PROGRESS_IN_ERROR`` - The provisioned product is under change but the requested operation failed and some remediation is occurring. For example, a rollback.

             

             ``SUCCEEDED`` - The requested operation has successfully completed.

             

             ``FAILED`` - The requested operation has completed but has failed. Investigate using the error messages returned.

            
          

          - **CreatedTime** *(datetime) --* 

            The UTC timestamp of the creation time.

            
          

          - **UpdatedTime** *(datetime) --* 

            The time when the record for the ProvisionedProduct object was last updated.

            
          

          - **ProvisionedProductType** *(string) --* 

            The type of the ProvisionedProduct object.

            
          

          - **RecordType** *(string) --* 

            The record type for this record.

            
          

          - **ProvisionedProductId** *(string) --* 

            The identifier of the ProvisionedProduct object.

            
          

          - **ProductId** *(string) --* 

            The product identifier.

            
          

          - **ProvisioningArtifactId** *(string) --* 

            The provisioning artifact identifier for this product. This is sometimes referred to as the product version.

            
          

          - **PathId** *(string) --* 

            The identifier of the path for this product's provisioning.

            
          

          - **RecordErrors** *(list) --* 

            A list of errors that occurred while processing the request.

            
            

            - *(dict) --* 

              The error code and description resulting from an operation.

              
              

              - **Code** *(string) --* 

                The numeric value of the error.

                
              

              - **Description** *(string) --* 

                The text description of the error.

                
          
        
          

          - **RecordTags** *(list) --* 

            List of tags associated with this record.

            
            

            - *(dict) --* 

              A tag associated with the record, stored as a key-value pair.

              
              

              - **Key** *(string) --* 

                The key for this tag.

                
              

              - **Value** *(string) --* 

                The value for this tag.

                
          
        
      
    

  .. py:method:: update_constraint(**kwargs)

    

    Updates an existing constraint.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/UpdateConstraint>`_    


    **Request Syntax** 
    ::

      response = client.update_constraint(
          AcceptLanguage='string',
          Id='string',
          Description='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type Id: string
    :param Id: **[REQUIRED]** 

      The identifier of the constraint to update.

      

    
    :type Description: string
    :param Description: 

      The updated text description of the constraint.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ConstraintDetail': {
                'ConstraintId': 'string',
                'Type': 'string',
                'Description': 'string',
                'Owner': 'string'
            },
            'ConstraintParameters': 'string',
            'Status': 'AVAILABLE'|'CREATING'|'FAILED'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ConstraintDetail** *(dict) --* 

          The resulting detailed constraint information.

          
          

          - **ConstraintId** *(string) --* 

            The identifier of the constraint.

            
          

          - **Type** *(string) --* 

            The type of the constraint.

            
          

          - **Description** *(string) --* 

            The text description of the constraint.

            
          

          - **Owner** *(string) --* 

            The owner of the constraint.

            
      
        

        - **ConstraintParameters** *(string) --* 

          The resulting updated constraint parameters.

          
        

        - **Status** *(string) --* 

          The status of the current request.

          
    

  .. py:method:: update_portfolio(**kwargs)

    

    Updates the specified portfolio's details. This operation does not work with a product that has been shared with you.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/UpdatePortfolio>`_    


    **Request Syntax** 
    ::

      response = client.update_portfolio(
          AcceptLanguage='string',
          Id='string',
          DisplayName='string',
          Description='string',
          ProviderName='string',
          AddTags=[
              {
                  'Key': 'string',
                  'Value': 'string'
              },
          ],
          RemoveTags=[
              'string',
          ]
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type Id: string
    :param Id: **[REQUIRED]** 

      The identifier of the portfolio for the update request.

      

    
    :type DisplayName: string
    :param DisplayName: 

      The name to use for display purposes.

      

    
    :type Description: string
    :param Description: 

      The updated text description of the portfolio.

      

    
    :type ProviderName: string
    :param ProviderName: 

      The updated name of the portfolio provider.

      

    
    :type AddTags: list
    :param AddTags: 

      Tags to add to the existing list of tags associated with the portfolio.

      

    
      - *(dict) --* 

        Key-value pairs to associate with this provisioning. These tags are entirely discretionary and are propagated to the resources created in the provisioning.

        

      
        - **Key** *(string) --* **[REQUIRED]** 

          The ``ProvisioningArtifactParameter.TagKey`` parameter from  DescribeProvisioningParameters .

          

        
        - **Value** *(string) --* **[REQUIRED]** 

          The desired value for this key.

          

        
      
  
    :type RemoveTags: list
    :param RemoveTags: 

      Tags to remove from the existing list of tags associated with the portfolio.

      

    
      - *(string) --* 

      
  
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'PortfolioDetail': {
                'Id': 'string',
                'ARN': 'string',
                'DisplayName': 'string',
                'Description': 'string',
                'CreatedTime': datetime(2015, 1, 1),
                'ProviderName': 'string'
            },
            'Tags': [
                {
                    'Key': 'string',
                    'Value': 'string'
                },
            ]
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **PortfolioDetail** *(dict) --* 

          The resulting detailed portfolio information.

          
          

          - **Id** *(string) --* 

            The identifier for the portfolio.

            
          

          - **ARN** *(string) --* 

            The ARN assigned to the portfolio.

            
          

          - **DisplayName** *(string) --* 

            The name to use for display purposes.

            
          

          - **Description** *(string) --* 

            The text description of the portfolio.

            
          

          - **CreatedTime** *(datetime) --* 

            The UTC timestamp of the creation time.

            
          

          - **ProviderName** *(string) --* 

            The name of the portfolio provider.

            
      
        

        - **Tags** *(list) --* 

          Tags associated with the portfolio.

          
          

          - *(dict) --* 

            Key-value pairs to associate with this provisioning. These tags are entirely discretionary and are propagated to the resources created in the provisioning.

            
            

            - **Key** *(string) --* 

              The ``ProvisioningArtifactParameter.TagKey`` parameter from  DescribeProvisioningParameters .

              
            

            - **Value** *(string) --* 

              The desired value for this key.

              
        
      
    

  .. py:method:: update_product(**kwargs)

    

    Updates an existing product.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/UpdateProduct>`_    


    **Request Syntax** 
    ::

      response = client.update_product(
          AcceptLanguage='string',
          Id='string',
          Name='string',
          Owner='string',
          Description='string',
          Distributor='string',
          SupportDescription='string',
          SupportEmail='string',
          SupportUrl='string',
          AddTags=[
              {
                  'Key': 'string',
                  'Value': 'string'
              },
          ],
          RemoveTags=[
              'string',
          ]
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type Id: string
    :param Id: **[REQUIRED]** 

      The identifier of the product for the update request.

      

    
    :type Name: string
    :param Name: 

      The updated product name.

      

    
    :type Owner: string
    :param Owner: 

      The updated owner of the product.

      

    
    :type Description: string
    :param Description: 

      The updated text description of the product.

      

    
    :type Distributor: string
    :param Distributor: 

      The updated distributor of the product.

      

    
    :type SupportDescription: string
    :param SupportDescription: 

      The updated support description for the product.

      

    
    :type SupportEmail: string
    :param SupportEmail: 

      The updated support email for the product.

      

    
    :type SupportUrl: string
    :param SupportUrl: 

      The updated support URL for the product.

      

    
    :type AddTags: list
    :param AddTags: 

      Tags to add to the existing list of tags associated with the product.

      

    
      - *(dict) --* 

        Key-value pairs to associate with this provisioning. These tags are entirely discretionary and are propagated to the resources created in the provisioning.

        

      
        - **Key** *(string) --* **[REQUIRED]** 

          The ``ProvisioningArtifactParameter.TagKey`` parameter from  DescribeProvisioningParameters .

          

        
        - **Value** *(string) --* **[REQUIRED]** 

          The desired value for this key.

          

        
      
  
    :type RemoveTags: list
    :param RemoveTags: 

      Tags to remove from the existing list of tags associated with the product.

      

    
      - *(string) --* 

      
  
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ProductViewDetail': {
                'ProductViewSummary': {
                    'Id': 'string',
                    'ProductId': 'string',
                    'Name': 'string',
                    'Owner': 'string',
                    'ShortDescription': 'string',
                    'Type': 'CLOUD_FORMATION_TEMPLATE'|'MARKETPLACE',
                    'Distributor': 'string',
                    'HasDefaultPath': True|False,
                    'SupportEmail': 'string',
                    'SupportDescription': 'string',
                    'SupportUrl': 'string'
                },
                'Status': 'AVAILABLE'|'CREATING'|'FAILED',
                'ProductARN': 'string',
                'CreatedTime': datetime(2015, 1, 1)
            },
            'Tags': [
                {
                    'Key': 'string',
                    'Value': 'string'
                },
            ]
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ProductViewDetail** *(dict) --* 

          The resulting detailed product view information.

          
          

          - **ProductViewSummary** *(dict) --* 

            The summary metadata about the specified product view.

            
            

            - **Id** *(string) --* 

              The product view identifier.

              
            

            - **ProductId** *(string) --* 

              The product identifier.

              
            

            - **Name** *(string) --* 

              The name of the product.

              
            

            - **Owner** *(string) --* 

              The owner of the product. Contact the product administrator for the significance of this value.

              
            

            - **ShortDescription** *(string) --* 

              Short description of the product.

              
            

            - **Type** *(string) --* 

              The product type. Contact the product administrator for the significance of this value. If this value is ``MARKETPLACE`` , the product was created by AWS Marketplace.

              
            

            - **Distributor** *(string) --* 

              The distributor of the product. Contact the product administrator for the significance of this value.

              
            

            - **HasDefaultPath** *(boolean) --* 

              A value of ``false`` indicates that the product does not have a default path, while a value of ``true`` indicates that it does. If it's false, call  ListLaunchPaths to disambiguate between paths. If true,  ListLaunchPaths is not required, and the output of the  ProductViewSummary operation can be used directly with  DescribeProvisioningParameters .

              
            

            - **SupportEmail** *(string) --* 

              The email contact information to obtain support for this Product.

              
            

            - **SupportDescription** *(string) --* 

              The description of the support for this Product.

              
            

            - **SupportUrl** *(string) --* 

              The URL information to obtain support for this Product.

              
        
          

          - **Status** *(string) --* 

            Current status of the product.

             

             ``AVAILABLE`` - Product is available for use.

             

             ``CREATING`` - Creation of product started, not ready for use.

             

             ``FAILED`` - Action on product failed.

            
          

          - **ProductARN** *(string) --* 

            The ARN associated with the product.

            
          

          - **CreatedTime** *(datetime) --* 

            The UTC timestamp of the creation time.

            
      
        

        - **Tags** *(list) --* 

          Tags associated with the product.

          
          

          - *(dict) --* 

            Key-value pairs to associate with this provisioning. These tags are entirely discretionary and are propagated to the resources created in the provisioning.

            
            

            - **Key** *(string) --* 

              The ``ProvisioningArtifactParameter.TagKey`` parameter from  DescribeProvisioningParameters .

              
            

            - **Value** *(string) --* 

              The desired value for this key.

              
        
      
    

  .. py:method:: update_provisioned_product(**kwargs)

    

    Requests updates to the configuration of an existing ProvisionedProduct object. If there are tags associated with the object, they cannot be updated or added with this operation. Depending on the specific updates requested, this operation may update with no interruption, with some interruption, or replace the ProvisionedProduct object entirely. 

     

    You can check the status of this request using the  DescribeRecord operation.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/UpdateProvisionedProduct>`_    


    **Request Syntax** 
    ::

      response = client.update_provisioned_product(
          AcceptLanguage='string',
          ProvisionedProductName='string',
          ProvisionedProductId='string',
          ProductId='string',
          ProvisioningArtifactId='string',
          PathId='string',
          ProvisioningParameters=[
              {
                  'Key': 'string',
                  'Value': 'string',
                  'UsePreviousValue': True|False
              },
          ],
          UpdateToken='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type ProvisionedProductName: string
    :param ProvisionedProductName: 

      The updated name of the ProvisionedProduct object. Specify either ``ProvisionedProductName`` or ``ProvisionedProductId`` , but not both.

      

    
    :type ProvisionedProductId: string
    :param ProvisionedProductId: 

      The identifier of the ProvisionedProduct object to update. Specify either ``ProvisionedProductName`` or ``ProvisionedProductId`` , but not both.

      

    
    :type ProductId: string
    :param ProductId: 

      The identifier of the ProvisionedProduct object.

      

    
    :type ProvisioningArtifactId: string
    :param ProvisioningArtifactId: 

      The provisioning artifact identifier for this product. This is sometimes referred to as the product version.

      

    
    :type PathId: string
    :param PathId: 

      The identifier of the path to use in the updated ProvisionedProduct object. This value is optional if the product has a default path, and is required if there is more than one path for the specified product.

      

    
    :type ProvisioningParameters: list
    :param ProvisioningParameters: 

      A list of ``ProvisioningParameter`` objects used to update the ProvisionedProduct object.

      

    
      - *(dict) --* 

        The parameter key-value pair used to update a ProvisionedProduct object. If ``UsePreviousValue`` is set to true, ``Value`` is ignored and the value for ``Key`` is kept as previously set (current value).

        

      
        - **Key** *(string) --* 

          The ``ProvisioningArtifactParameter.ParameterKey`` parameter from  DescribeProvisioningParameters .

          

        
        - **Value** *(string) --* 

          The value to use for updating the product provisioning. Any constraints on this value can be found in the ``ProvisioningArtifactParameter`` parameter for ``Key`` .

          

        
        - **UsePreviousValue** *(boolean) --* 

          If true, uses the currently set value for ``Key`` , ignoring ``UpdateProvisioningParameter.Value`` .

          

        
      
  
    :type UpdateToken: string
    :param UpdateToken: **[REQUIRED]** 

      The idempotency token that uniquely identifies the provisioning update request.

      This field is autopopulated if not provided.

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'RecordDetail': {
                'RecordId': 'string',
                'ProvisionedProductName': 'string',
                'Status': 'CREATED'|'IN_PROGRESS'|'IN_PROGRESS_IN_ERROR'|'SUCCEEDED'|'FAILED',
                'CreatedTime': datetime(2015, 1, 1),
                'UpdatedTime': datetime(2015, 1, 1),
                'ProvisionedProductType': 'string',
                'RecordType': 'string',
                'ProvisionedProductId': 'string',
                'ProductId': 'string',
                'ProvisioningArtifactId': 'string',
                'PathId': 'string',
                'RecordErrors': [
                    {
                        'Code': 'string',
                        'Description': 'string'
                    },
                ],
                'RecordTags': [
                    {
                        'Key': 'string',
                        'Value': 'string'
                    },
                ]
            }
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **RecordDetail** *(dict) --* 

          The detailed result of the  UpdateProvisionedProduct request, containing the inputs made to that request, the current state of the request, a pointer to the ProvisionedProduct object that the request is modifying, and a list of any errors that the request encountered.

          
          

          - **RecordId** *(string) --* 

            The identifier of the ProvisionedProduct object record.

            
          

          - **ProvisionedProductName** *(string) --* 

            The user-friendly name of the ProvisionedProduct object.

            
          

          - **Status** *(string) --* 

            The status of the ProvisionedProduct object.

             

             ``CREATED`` - Request created but the operation has not yet started.

             

             ``IN_PROGRESS`` - The requested operation is in-progress.

             

             ``IN_PROGRESS_IN_ERROR`` - The provisioned product is under change but the requested operation failed and some remediation is occurring. For example, a rollback.

             

             ``SUCCEEDED`` - The requested operation has successfully completed.

             

             ``FAILED`` - The requested operation has completed but has failed. Investigate using the error messages returned.

            
          

          - **CreatedTime** *(datetime) --* 

            The UTC timestamp of the creation time.

            
          

          - **UpdatedTime** *(datetime) --* 

            The time when the record for the ProvisionedProduct object was last updated.

            
          

          - **ProvisionedProductType** *(string) --* 

            The type of the ProvisionedProduct object.

            
          

          - **RecordType** *(string) --* 

            The record type for this record.

            
          

          - **ProvisionedProductId** *(string) --* 

            The identifier of the ProvisionedProduct object.

            
          

          - **ProductId** *(string) --* 

            The product identifier.

            
          

          - **ProvisioningArtifactId** *(string) --* 

            The provisioning artifact identifier for this product. This is sometimes referred to as the product version.

            
          

          - **PathId** *(string) --* 

            The identifier of the path for this product's provisioning.

            
          

          - **RecordErrors** *(list) --* 

            A list of errors that occurred while processing the request.

            
            

            - *(dict) --* 

              The error code and description resulting from an operation.

              
              

              - **Code** *(string) --* 

                The numeric value of the error.

                
              

              - **Description** *(string) --* 

                The text description of the error.

                
          
        
          

          - **RecordTags** *(list) --* 

            List of tags associated with this record.

            
            

            - *(dict) --* 

              A tag associated with the record, stored as a key-value pair.

              
              

              - **Key** *(string) --* 

                The key for this tag.

                
              

              - **Value** *(string) --* 

                The value for this tag.

                
          
        
      
    

  .. py:method:: update_provisioning_artifact(**kwargs)

    

    Updates an existing provisioning artifact's information. This operation does not work on a provisioning artifact associated with a product that has been shared with you.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/UpdateProvisioningArtifact>`_    


    **Request Syntax** 
    ::

      response = client.update_provisioning_artifact(
          AcceptLanguage='string',
          ProductId='string',
          ProvisioningArtifactId='string',
          Name='string',
          Description='string'
      )
    :type AcceptLanguage: string
    :param AcceptLanguage: 

      The language code.

       

       
      * ``en`` - English (default) 
       
      * ``jp`` - Japanese 
       
      * ``zh`` - Chinese 
       

      

    
    :type ProductId: string
    :param ProductId: **[REQUIRED]** 

      The product identifier.

      

    
    :type ProvisioningArtifactId: string
    :param ProvisioningArtifactId: **[REQUIRED]** 

      The identifier of the provisioning artifact for the update request. This is sometimes referred to as the product version.

      

    
    :type Name: string
    :param Name: 

      The updated name of the provisioning artifact.

      

    
    :type Description: string
    :param Description: 

      The updated text description of the provisioning artifact.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'ProvisioningArtifactDetail': {
                'Id': 'string',
                'Name': 'string',
                'Description': 'string',
                'Type': 'CLOUD_FORMATION_TEMPLATE'|'MARKETPLACE_AMI'|'MARKETPLACE_CAR',
                'CreatedTime': datetime(2015, 1, 1)
            },
            'Info': {
                'string': 'string'
            },
            'Status': 'AVAILABLE'|'CREATING'|'FAILED'
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **ProvisioningArtifactDetail** *(dict) --* 

          The resulting detailed provisioning artifact information.

          
          

          - **Id** *(string) --* 

            The identifier of the provisioning artifact. This is sometimes referred to as the product version.

            
          

          - **Name** *(string) --* 

            The name assigned to the provisioning artifact.

            
          

          - **Description** *(string) --* 

            The text description of the provisioning artifact.

            
          

          - **Type** *(string) --* 

            The type of the provisioning artifact. The following provisioning artifact types are used by AWS Marketplace products:

             

             ``MARKETPLACE_AMI`` - AMI products.

             

             ``MARKETPLACE_CAR`` - CAR (Cluster and AWS Resources) products.

            
          

          - **CreatedTime** *(datetime) --* 

            The UTC timestamp of the creation time.

            
      
        

        - **Info** *(dict) --* 

          Additional information about the provisioning artifact update request.

          
          

          - *(string) --* 
            

            - *(string) --* 
      
    
        

        - **Status** *(string) --* 

          The status of the current request.

          
    

  .. py:method:: update_tag_option(**kwargs)

    

    Updates an existing TagOption.

    

    See also: `AWS API Documentation <https://docs.aws.amazon.com/goto/WebAPI/servicecatalog-2015-12-10/UpdateTagOption>`_    


    **Request Syntax** 
    ::

      response = client.update_tag_option(
          Id='string',
          Value='string',
          Active=True|False
      )
    :type Id: string
    :param Id: **[REQUIRED]** 

      The identifier of the constraint to update.

      

    
    :type Value: string
    :param Value: 

      The updated value.

      

    
    :type Active: boolean
    :param Active: 

      The updated active state.

      

    
    
    :rtype: dict
    :returns: 
      
      **Response Syntax** 

      
      ::

        {
            'TagOptionDetail': {
                'Key': 'string',
                'Value': 'string',
                'Active': True|False,
                'Id': 'string'
            }
        }
      **Response Structure** 

      

      - *(dict) --* 
        

        - **TagOptionDetail** *(dict) --* 

          The resulting detailed TagOption information.

          
          

          - **Key** *(string) --* 

            The TagOptionDetail key.

            
          

          - **Value** *(string) --* 

            The TagOptionDetail value.

            
          

          - **Active** *(boolean) --* 

            The TagOptionDetail active state.

            
          

          - **Id** *(string) --* 

            The TagOptionDetail identifier.

            
      
    

==========
Paginators
==========


The available paginators are:
