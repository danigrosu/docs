---
title: "&lt;mexHttpBinding&gt;"
ms.date: "03/30/2017"
ms.assetid: e50b2e1f-9668-41a5-8077-dee7abff9f0f
---
# &lt;mexHttpBinding&gt;
Specifies the settings for a binding used for the WS-MetadataExchange (WS-MEX) message exchange over HTTP.  
  
 \<system.ServiceModel>  
\<bindings>  
\<mexHttpBinding>  
  
## Syntax  
  
```xml  
<mexHttpBinding>
  <binding closeTimeout="TimeSpan"
           name="string"
           openTimeout="TimeSpan"
           receiveTimeout="TimeSpan"
           sendTimeout="TimeSpan">
  </binding>
</mexHttpBinding>
```  
  
## Attributes and Elements  
 The following sections describe attributes, child elements, and parent elements.  
  
### Attributes  
  
|Attribute|Description|  
|---------------|-----------------|  
|`closeTimeout`|A <xref:System.TimeSpan> value that specifies the interval of time provided for a close operation to complete. This value should be greater than or equal to <xref:System.TimeSpan.Zero>. The default is 00:01:00.|  
|`name`|A string that contains the configuration name of the binding. This value should be unique because it is used as an identification for the binding. Each binding has a `name` and `namespace` attribute that together uniquely identify it in the metadata of the service. In addition, this name is unique among bindings of the same type. Starting with [!INCLUDE[netfx40_short](../../../../../includes/netfx40-short-md.md)], bindings and behaviors are not required to have a name. For more information about default configuration and nameless bindings and behaviors, see [Simplified Configuration](../../../../../docs/framework/wcf/simplified-configuration.md) and [Simplified Configuration for WCF Services](../../../../../docs/framework/wcf/samples/simplified-configuration-for-wcf-services.md).|  
|`openTimeout`|A <xref:System.TimeSpan> value that specifies the interval of time provided for an open operation to complete. This value should be greater than or equal to <xref:System.TimeSpan.Zero>. The default is 00:01:00.|  
|`receiveTimeout`|A <xref:System.TimeSpan> value that specifies the interval of time provided for a receive operation to complete. This value should be greater than or equal to <xref:System.TimeSpan.Zero>. The default is 00:10:00.|  
|`sendTimeout`|A <xref:System.TimeSpan> value that specifies the interval of time provided for a send operation to complete. This value should be greater than or equal to <xref:System.TimeSpan.Zero>. The default is 00:01:00.|  
  
### Child Elements  
 None.  
  
### Parent Elements  
  
|Element|Description|  
|-------------|-----------------|  
|[\<bindings>](../../../../../docs/framework/configure-apps/file-schema/wcf/bindings.md)|This element holds a collection of standard and custom bindings.|  
  
## Remarks  
 This binding is essentially a `WSHttpBinding` binding with security disabled. It supports most metadata requests.  
  
## See Also  
 <xref:System.ServiceModel.Description.MetadataExchangeBindings.CreateMexHttpBinding%2A>  
 <xref:System.ServiceModel.Configuration.MexHttpBindingElement>  
 [How to: Publish Metadata for a Service Using a Configuration File](../../../../../docs/framework/wcf/feature-details/how-to-publish-metadata-for-a-service-using-a-configuration-file.md)  
 [Publishing and Retrieving Metadata Over a Custom Binding](../../../../../docs/framework/wcf/extending/publishing-and-retrieving-metadata-over-a-custom-binding.md)  
 [Metadata](../../../../../docs/framework/wcf/feature-details/metadata.md)  
 [Bindings](../../../../../docs/framework/wcf/bindings.md)  
 [Configuring System-Provided Bindings](../../../../../docs/framework/wcf/feature-details/configuring-system-provided-bindings.md)  
 [Using Bindings to Configure Services and Clients](../../../../../docs/framework/wcf/using-bindings-to-configure-services-and-clients.md)  
 [\<binding>](../../../../../docs/framework/misc/binding.md)
