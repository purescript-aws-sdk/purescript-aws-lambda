## Module AWS.Lambda.Types

#### `options`

``` purescript
options :: Options
```

#### `AddEventSourceRequest`

``` purescript
newtype AddEventSourceRequest
  = AddEventSourceRequest { "EventSource" :: String, "FunctionName" :: FunctionName, "Role" :: RoleArn, "BatchSize" :: Maybe (Int), "Parameters" :: Maybe (Map'') }
```

##### Instances
``` purescript
Newtype AddEventSourceRequest _
Generic AddEventSourceRequest _
Show AddEventSourceRequest
Decode AddEventSourceRequest
Encode AddEventSourceRequest
```

#### `newAddEventSourceRequest`

``` purescript
newAddEventSourceRequest :: String -> FunctionName -> RoleArn -> AddEventSourceRequest
```

Constructs AddEventSourceRequest from required parameters

#### `newAddEventSourceRequest'`

``` purescript
newAddEventSourceRequest' :: String -> FunctionName -> RoleArn -> ({ "EventSource" :: String, "FunctionName" :: FunctionName, "Role" :: RoleArn, "BatchSize" :: Maybe (Int), "Parameters" :: Maybe (Map'') } -> { "EventSource" :: String, "FunctionName" :: FunctionName, "Role" :: RoleArn, "BatchSize" :: Maybe (Int), "Parameters" :: Maybe (Map'') }) -> AddEventSourceRequest
```

Constructs AddEventSourceRequest's fields from required parameters

#### `DeleteFunctionRequest`

``` purescript
newtype DeleteFunctionRequest
  = DeleteFunctionRequest { "FunctionName" :: FunctionName }
```

##### Instances
``` purescript
Newtype DeleteFunctionRequest _
Generic DeleteFunctionRequest _
Show DeleteFunctionRequest
Decode DeleteFunctionRequest
Encode DeleteFunctionRequest
```

#### `newDeleteFunctionRequest`

``` purescript
newDeleteFunctionRequest :: FunctionName -> DeleteFunctionRequest
```

Constructs DeleteFunctionRequest from required parameters

#### `newDeleteFunctionRequest'`

``` purescript
newDeleteFunctionRequest' :: FunctionName -> ({ "FunctionName" :: FunctionName } -> { "FunctionName" :: FunctionName }) -> DeleteFunctionRequest
```

Constructs DeleteFunctionRequest's fields from required parameters

#### `Description`

``` purescript
newtype Description
  = Description String
```

##### Instances
``` purescript
Newtype Description _
Generic Description _
Show Description
Decode Description
Encode Description
```

#### `EventSourceConfiguration`

``` purescript
newtype EventSourceConfiguration
  = EventSourceConfiguration { "UUID" :: Maybe (String), "BatchSize" :: Maybe (Int), "EventSource" :: Maybe (String), "FunctionName" :: Maybe (FunctionName), "Parameters" :: Maybe (Map''), "Role" :: Maybe (RoleArn), "LastModified" :: Maybe (Timestamp), "IsActive" :: Maybe (Boolean), "Status" :: Maybe (String) }
```

<p>Describes mapping between an Amazon Kinesis stream and a Lambda function.</p>

##### Instances
``` purescript
Newtype EventSourceConfiguration _
Generic EventSourceConfiguration _
Show EventSourceConfiguration
Decode EventSourceConfiguration
Encode EventSourceConfiguration
```

#### `newEventSourceConfiguration`

``` purescript
newEventSourceConfiguration :: EventSourceConfiguration
```

Constructs EventSourceConfiguration from required parameters

#### `newEventSourceConfiguration'`

``` purescript
newEventSourceConfiguration' :: ({ "UUID" :: Maybe (String), "BatchSize" :: Maybe (Int), "EventSource" :: Maybe (String), "FunctionName" :: Maybe (FunctionName), "Parameters" :: Maybe (Map''), "Role" :: Maybe (RoleArn), "LastModified" :: Maybe (Timestamp), "IsActive" :: Maybe (Boolean), "Status" :: Maybe (String) } -> { "UUID" :: Maybe (String), "BatchSize" :: Maybe (Int), "EventSource" :: Maybe (String), "FunctionName" :: Maybe (FunctionName), "Parameters" :: Maybe (Map''), "Role" :: Maybe (RoleArn), "LastModified" :: Maybe (Timestamp), "IsActive" :: Maybe (Boolean), "Status" :: Maybe (String) }) -> EventSourceConfiguration
```

Constructs EventSourceConfiguration's fields from required parameters

#### `EventSourceList`

``` purescript
newtype EventSourceList
  = EventSourceList (Array EventSourceConfiguration)
```

##### Instances
``` purescript
Newtype EventSourceList _
Generic EventSourceList _
Show EventSourceList
Decode EventSourceList
Encode EventSourceList
```

#### `FunctionArn`

``` purescript
newtype FunctionArn
  = FunctionArn String
```

##### Instances
``` purescript
Newtype FunctionArn _
Generic FunctionArn _
Show FunctionArn
Decode FunctionArn
Encode FunctionArn
```

#### `FunctionCodeLocation`

``` purescript
newtype FunctionCodeLocation
  = FunctionCodeLocation { "RepositoryType" :: Maybe (String), "Location" :: Maybe (String) }
```

<p>The object for the Lambda function location.</p>

##### Instances
``` purescript
Newtype FunctionCodeLocation _
Generic FunctionCodeLocation _
Show FunctionCodeLocation
Decode FunctionCodeLocation
Encode FunctionCodeLocation
```

#### `newFunctionCodeLocation`

``` purescript
newFunctionCodeLocation :: FunctionCodeLocation
```

Constructs FunctionCodeLocation from required parameters

#### `newFunctionCodeLocation'`

``` purescript
newFunctionCodeLocation' :: ({ "RepositoryType" :: Maybe (String), "Location" :: Maybe (String) } -> { "RepositoryType" :: Maybe (String), "Location" :: Maybe (String) }) -> FunctionCodeLocation
```

Constructs FunctionCodeLocation's fields from required parameters

#### `FunctionConfiguration`

``` purescript
newtype FunctionConfiguration
  = FunctionConfiguration { "FunctionName" :: Maybe (FunctionName), "FunctionARN" :: Maybe (FunctionArn), "ConfigurationId" :: Maybe (String), "Runtime" :: Maybe (Runtime), "Role" :: Maybe (RoleArn), "Handler" :: Maybe (Handler), "Mode" :: Maybe (Mode), "CodeSize" :: Maybe (Number), "Description" :: Maybe (Description), "Timeout" :: Maybe (Timeout), "MemorySize" :: Maybe (MemorySize), "LastModified" :: Maybe (Timestamp) }
```

<p>A complex type that describes function metadata.</p>

##### Instances
``` purescript
Newtype FunctionConfiguration _
Generic FunctionConfiguration _
Show FunctionConfiguration
Decode FunctionConfiguration
Encode FunctionConfiguration
```

#### `newFunctionConfiguration`

``` purescript
newFunctionConfiguration :: FunctionConfiguration
```

Constructs FunctionConfiguration from required parameters

#### `newFunctionConfiguration'`

``` purescript
newFunctionConfiguration' :: ({ "FunctionName" :: Maybe (FunctionName), "FunctionARN" :: Maybe (FunctionArn), "ConfigurationId" :: Maybe (String), "Runtime" :: Maybe (Runtime), "Role" :: Maybe (RoleArn), "Handler" :: Maybe (Handler), "Mode" :: Maybe (Mode), "CodeSize" :: Maybe (Number), "Description" :: Maybe (Description), "Timeout" :: Maybe (Timeout), "MemorySize" :: Maybe (MemorySize), "LastModified" :: Maybe (Timestamp) } -> { "FunctionName" :: Maybe (FunctionName), "FunctionARN" :: Maybe (FunctionArn), "ConfigurationId" :: Maybe (String), "Runtime" :: Maybe (Runtime), "Role" :: Maybe (RoleArn), "Handler" :: Maybe (Handler), "Mode" :: Maybe (Mode), "CodeSize" :: Maybe (Number), "Description" :: Maybe (Description), "Timeout" :: Maybe (Timeout), "MemorySize" :: Maybe (MemorySize), "LastModified" :: Maybe (Timestamp) }) -> FunctionConfiguration
```

Constructs FunctionConfiguration's fields from required parameters

#### `FunctionList`

``` purescript
newtype FunctionList
  = FunctionList (Array FunctionConfiguration)
```

##### Instances
``` purescript
Newtype FunctionList _
Generic FunctionList _
Show FunctionList
Decode FunctionList
Encode FunctionList
```

#### `FunctionName`

``` purescript
newtype FunctionName
  = FunctionName String
```

##### Instances
``` purescript
Newtype FunctionName _
Generic FunctionName _
Show FunctionName
Decode FunctionName
Encode FunctionName
```

#### `GetEventSourceRequest`

``` purescript
newtype GetEventSourceRequest
  = GetEventSourceRequest { "UUID" :: String }
```

##### Instances
``` purescript
Newtype GetEventSourceRequest _
Generic GetEventSourceRequest _
Show GetEventSourceRequest
Decode GetEventSourceRequest
Encode GetEventSourceRequest
```

#### `newGetEventSourceRequest`

``` purescript
newGetEventSourceRequest :: String -> GetEventSourceRequest
```

Constructs GetEventSourceRequest from required parameters

#### `newGetEventSourceRequest'`

``` purescript
newGetEventSourceRequest' :: String -> ({ "UUID" :: String } -> { "UUID" :: String }) -> GetEventSourceRequest
```

Constructs GetEventSourceRequest's fields from required parameters

#### `GetFunctionConfigurationRequest`

``` purescript
newtype GetFunctionConfigurationRequest
  = GetFunctionConfigurationRequest { "FunctionName" :: FunctionName }
```

##### Instances
``` purescript
Newtype GetFunctionConfigurationRequest _
Generic GetFunctionConfigurationRequest _
Show GetFunctionConfigurationRequest
Decode GetFunctionConfigurationRequest
Encode GetFunctionConfigurationRequest
```

#### `newGetFunctionConfigurationRequest`

``` purescript
newGetFunctionConfigurationRequest :: FunctionName -> GetFunctionConfigurationRequest
```

Constructs GetFunctionConfigurationRequest from required parameters

#### `newGetFunctionConfigurationRequest'`

``` purescript
newGetFunctionConfigurationRequest' :: FunctionName -> ({ "FunctionName" :: FunctionName } -> { "FunctionName" :: FunctionName }) -> GetFunctionConfigurationRequest
```

Constructs GetFunctionConfigurationRequest's fields from required parameters

#### `GetFunctionRequest`

``` purescript
newtype GetFunctionRequest
  = GetFunctionRequest { "FunctionName" :: FunctionName }
```

##### Instances
``` purescript
Newtype GetFunctionRequest _
Generic GetFunctionRequest _
Show GetFunctionRequest
Decode GetFunctionRequest
Encode GetFunctionRequest
```

#### `newGetFunctionRequest`

``` purescript
newGetFunctionRequest :: FunctionName -> GetFunctionRequest
```

Constructs GetFunctionRequest from required parameters

#### `newGetFunctionRequest'`

``` purescript
newGetFunctionRequest' :: FunctionName -> ({ "FunctionName" :: FunctionName } -> { "FunctionName" :: FunctionName }) -> GetFunctionRequest
```

Constructs GetFunctionRequest's fields from required parameters

#### `GetFunctionResponse`

``` purescript
newtype GetFunctionResponse
  = GetFunctionResponse { "Configuration" :: Maybe (FunctionConfiguration), "Code" :: Maybe (FunctionCodeLocation) }
```

<p>This response contains the object for AWS Lambda function location (see <a>API_FunctionCodeLocation</a></p>

##### Instances
``` purescript
Newtype GetFunctionResponse _
Generic GetFunctionResponse _
Show GetFunctionResponse
Decode GetFunctionResponse
Encode GetFunctionResponse
```

#### `newGetFunctionResponse`

``` purescript
newGetFunctionResponse :: GetFunctionResponse
```

Constructs GetFunctionResponse from required parameters

#### `newGetFunctionResponse'`

``` purescript
newGetFunctionResponse' :: ({ "Configuration" :: Maybe (FunctionConfiguration), "Code" :: Maybe (FunctionCodeLocation) } -> { "Configuration" :: Maybe (FunctionConfiguration), "Code" :: Maybe (FunctionCodeLocation) }) -> GetFunctionResponse
```

Constructs GetFunctionResponse's fields from required parameters

#### `Handler`

``` purescript
newtype Handler
  = Handler String
```

##### Instances
``` purescript
Newtype Handler _
Generic Handler _
Show Handler
Decode Handler
Encode Handler
```

#### `HttpStatus`

``` purescript
newtype HttpStatus
  = HttpStatus Int
```

##### Instances
``` purescript
Newtype HttpStatus _
Generic HttpStatus _
Show HttpStatus
Decode HttpStatus
Encode HttpStatus
```

#### `InvalidParameterValueException`

``` purescript
newtype InvalidParameterValueException
  = InvalidParameterValueException { "Type" :: Maybe (String), message :: Maybe (String) }
```

<p>One of the parameters in the request is invalid. For example, if you provided an IAM role for AWS Lambda to assume in the <code>UploadFunction</code> or the <code>UpdateFunctionConfiguration</code> API, that AWS Lambda is unable to assume you will get this exception. </p>

##### Instances
``` purescript
Newtype InvalidParameterValueException _
Generic InvalidParameterValueException _
Show InvalidParameterValueException
Decode InvalidParameterValueException
Encode InvalidParameterValueException
```

#### `newInvalidParameterValueException`

``` purescript
newInvalidParameterValueException :: InvalidParameterValueException
```

Constructs InvalidParameterValueException from required parameters

#### `newInvalidParameterValueException'`

``` purescript
newInvalidParameterValueException' :: ({ "Type" :: Maybe (String), message :: Maybe (String) } -> { "Type" :: Maybe (String), message :: Maybe (String) }) -> InvalidParameterValueException
```

Constructs InvalidParameterValueException's fields from required parameters

#### `InvalidRequestContentException`

``` purescript
newtype InvalidRequestContentException
  = InvalidRequestContentException { "Type" :: Maybe (String), message :: Maybe (String) }
```

<p>The request body could not be parsed as JSON.</p>

##### Instances
``` purescript
Newtype InvalidRequestContentException _
Generic InvalidRequestContentException _
Show InvalidRequestContentException
Decode InvalidRequestContentException
Encode InvalidRequestContentException
```

#### `newInvalidRequestContentException`

``` purescript
newInvalidRequestContentException :: InvalidRequestContentException
```

Constructs InvalidRequestContentException from required parameters

#### `newInvalidRequestContentException'`

``` purescript
newInvalidRequestContentException' :: ({ "Type" :: Maybe (String), message :: Maybe (String) } -> { "Type" :: Maybe (String), message :: Maybe (String) }) -> InvalidRequestContentException
```

Constructs InvalidRequestContentException's fields from required parameters

#### `InvokeAsyncRequest`

``` purescript
newtype InvokeAsyncRequest
  = InvokeAsyncRequest { "FunctionName" :: FunctionName, "InvokeArgs" :: String }
```

##### Instances
``` purescript
Newtype InvokeAsyncRequest _
Generic InvokeAsyncRequest _
Show InvokeAsyncRequest
Decode InvokeAsyncRequest
Encode InvokeAsyncRequest
```

#### `newInvokeAsyncRequest`

``` purescript
newInvokeAsyncRequest :: FunctionName -> String -> InvokeAsyncRequest
```

Constructs InvokeAsyncRequest from required parameters

#### `newInvokeAsyncRequest'`

``` purescript
newInvokeAsyncRequest' :: FunctionName -> String -> ({ "FunctionName" :: FunctionName, "InvokeArgs" :: String } -> { "FunctionName" :: FunctionName, "InvokeArgs" :: String }) -> InvokeAsyncRequest
```

Constructs InvokeAsyncRequest's fields from required parameters

#### `InvokeAsyncResponse`

``` purescript
newtype InvokeAsyncResponse
  = InvokeAsyncResponse { "Status" :: Maybe (HttpStatus) }
```

<p>Upon success, it returns empty response. Otherwise, throws an exception.</p>

##### Instances
``` purescript
Newtype InvokeAsyncResponse _
Generic InvokeAsyncResponse _
Show InvokeAsyncResponse
Decode InvokeAsyncResponse
Encode InvokeAsyncResponse
```

#### `newInvokeAsyncResponse`

``` purescript
newInvokeAsyncResponse :: InvokeAsyncResponse
```

Constructs InvokeAsyncResponse from required parameters

#### `newInvokeAsyncResponse'`

``` purescript
newInvokeAsyncResponse' :: ({ "Status" :: Maybe (HttpStatus) } -> { "Status" :: Maybe (HttpStatus) }) -> InvokeAsyncResponse
```

Constructs InvokeAsyncResponse's fields from required parameters

#### `ListEventSourcesRequest`

``` purescript
newtype ListEventSourcesRequest
  = ListEventSourcesRequest { "EventSourceArn" :: Maybe (String), "FunctionName" :: Maybe (FunctionName), "Marker" :: Maybe (String), "MaxItems" :: Maybe (MaxListItems) }
```

##### Instances
``` purescript
Newtype ListEventSourcesRequest _
Generic ListEventSourcesRequest _
Show ListEventSourcesRequest
Decode ListEventSourcesRequest
Encode ListEventSourcesRequest
```

#### `newListEventSourcesRequest`

``` purescript
newListEventSourcesRequest :: ListEventSourcesRequest
```

Constructs ListEventSourcesRequest from required parameters

#### `newListEventSourcesRequest'`

``` purescript
newListEventSourcesRequest' :: ({ "EventSourceArn" :: Maybe (String), "FunctionName" :: Maybe (FunctionName), "Marker" :: Maybe (String), "MaxItems" :: Maybe (MaxListItems) } -> { "EventSourceArn" :: Maybe (String), "FunctionName" :: Maybe (FunctionName), "Marker" :: Maybe (String), "MaxItems" :: Maybe (MaxListItems) }) -> ListEventSourcesRequest
```

Constructs ListEventSourcesRequest's fields from required parameters

#### `ListEventSourcesResponse`

``` purescript
newtype ListEventSourcesResponse
  = ListEventSourcesResponse { "NextMarker" :: Maybe (String), "EventSources" :: Maybe (EventSourceList) }
```

<p>Contains a list of event sources (see <a>API_EventSourceConfiguration</a>)</p>

##### Instances
``` purescript
Newtype ListEventSourcesResponse _
Generic ListEventSourcesResponse _
Show ListEventSourcesResponse
Decode ListEventSourcesResponse
Encode ListEventSourcesResponse
```

#### `newListEventSourcesResponse`

``` purescript
newListEventSourcesResponse :: ListEventSourcesResponse
```

Constructs ListEventSourcesResponse from required parameters

#### `newListEventSourcesResponse'`

``` purescript
newListEventSourcesResponse' :: ({ "NextMarker" :: Maybe (String), "EventSources" :: Maybe (EventSourceList) } -> { "NextMarker" :: Maybe (String), "EventSources" :: Maybe (EventSourceList) }) -> ListEventSourcesResponse
```

Constructs ListEventSourcesResponse's fields from required parameters

#### `ListFunctionsRequest`

``` purescript
newtype ListFunctionsRequest
  = ListFunctionsRequest { "Marker" :: Maybe (String), "MaxItems" :: Maybe (MaxListItems) }
```

##### Instances
``` purescript
Newtype ListFunctionsRequest _
Generic ListFunctionsRequest _
Show ListFunctionsRequest
Decode ListFunctionsRequest
Encode ListFunctionsRequest
```

#### `newListFunctionsRequest`

``` purescript
newListFunctionsRequest :: ListFunctionsRequest
```

Constructs ListFunctionsRequest from required parameters

#### `newListFunctionsRequest'`

``` purescript
newListFunctionsRequest' :: ({ "Marker" :: Maybe (String), "MaxItems" :: Maybe (MaxListItems) } -> { "Marker" :: Maybe (String), "MaxItems" :: Maybe (MaxListItems) }) -> ListFunctionsRequest
```

Constructs ListFunctionsRequest's fields from required parameters

#### `ListFunctionsResponse`

``` purescript
newtype ListFunctionsResponse
  = ListFunctionsResponse { "NextMarker" :: Maybe (String), "Functions" :: Maybe (FunctionList) }
```

<p>Contains a list of AWS Lambda function configurations (see <a>API_FunctionConfiguration</a>.</p>

##### Instances
``` purescript
Newtype ListFunctionsResponse _
Generic ListFunctionsResponse _
Show ListFunctionsResponse
Decode ListFunctionsResponse
Encode ListFunctionsResponse
```

#### `newListFunctionsResponse`

``` purescript
newListFunctionsResponse :: ListFunctionsResponse
```

Constructs ListFunctionsResponse from required parameters

#### `newListFunctionsResponse'`

``` purescript
newListFunctionsResponse' :: ({ "NextMarker" :: Maybe (String), "Functions" :: Maybe (FunctionList) } -> { "NextMarker" :: Maybe (String), "Functions" :: Maybe (FunctionList) }) -> ListFunctionsResponse
```

Constructs ListFunctionsResponse's fields from required parameters

#### `Map''`

``` purescript
newtype Map''
  = Map'' (StrMap String)
```

##### Instances
``` purescript
Newtype Map'' _
Generic Map'' _
Show Map''
Decode Map''
Encode Map''
```

#### `MaxListItems`

``` purescript
newtype MaxListItems
  = MaxListItems Int
```

##### Instances
``` purescript
Newtype MaxListItems _
Generic MaxListItems _
Show MaxListItems
Decode MaxListItems
Encode MaxListItems
```

#### `MemorySize`

``` purescript
newtype MemorySize
  = MemorySize Int
```

##### Instances
``` purescript
Newtype MemorySize _
Generic MemorySize _
Show MemorySize
Decode MemorySize
Encode MemorySize
```

#### `Mode`

``` purescript
newtype Mode
  = Mode String
```

##### Instances
``` purescript
Newtype Mode _
Generic Mode _
Show Mode
Decode Mode
Encode Mode
```

#### `RemoveEventSourceRequest`

``` purescript
newtype RemoveEventSourceRequest
  = RemoveEventSourceRequest { "UUID" :: String }
```

##### Instances
``` purescript
Newtype RemoveEventSourceRequest _
Generic RemoveEventSourceRequest _
Show RemoveEventSourceRequest
Decode RemoveEventSourceRequest
Encode RemoveEventSourceRequest
```

#### `newRemoveEventSourceRequest`

``` purescript
newRemoveEventSourceRequest :: String -> RemoveEventSourceRequest
```

Constructs RemoveEventSourceRequest from required parameters

#### `newRemoveEventSourceRequest'`

``` purescript
newRemoveEventSourceRequest' :: String -> ({ "UUID" :: String } -> { "UUID" :: String }) -> RemoveEventSourceRequest
```

Constructs RemoveEventSourceRequest's fields from required parameters

#### `ResourceNotFoundException`

``` purescript
newtype ResourceNotFoundException
  = ResourceNotFoundException { "Type" :: Maybe (String), "Message" :: Maybe (String) }
```

<p>The function or the event source specified in the request does not exist.</p>

##### Instances
``` purescript
Newtype ResourceNotFoundException _
Generic ResourceNotFoundException _
Show ResourceNotFoundException
Decode ResourceNotFoundException
Encode ResourceNotFoundException
```

#### `newResourceNotFoundException`

``` purescript
newResourceNotFoundException :: ResourceNotFoundException
```

Constructs ResourceNotFoundException from required parameters

#### `newResourceNotFoundException'`

``` purescript
newResourceNotFoundException' :: ({ "Type" :: Maybe (String), "Message" :: Maybe (String) } -> { "Type" :: Maybe (String), "Message" :: Maybe (String) }) -> ResourceNotFoundException
```

Constructs ResourceNotFoundException's fields from required parameters

#### `RoleArn`

``` purescript
newtype RoleArn
  = RoleArn String
```

##### Instances
``` purescript
Newtype RoleArn _
Generic RoleArn _
Show RoleArn
Decode RoleArn
Encode RoleArn
```

#### `Runtime`

``` purescript
newtype Runtime
  = Runtime String
```

##### Instances
``` purescript
Newtype Runtime _
Generic Runtime _
Show Runtime
Decode Runtime
Encode Runtime
```

#### `ServiceException`

``` purescript
newtype ServiceException
  = ServiceException { "Type" :: Maybe (String), "Message" :: Maybe (String) }
```

<p>The AWS Lambda service encountered an internal error.</p>

##### Instances
``` purescript
Newtype ServiceException _
Generic ServiceException _
Show ServiceException
Decode ServiceException
Encode ServiceException
```

#### `newServiceException`

``` purescript
newServiceException :: ServiceException
```

Constructs ServiceException from required parameters

#### `newServiceException'`

``` purescript
newServiceException' :: ({ "Type" :: Maybe (String), "Message" :: Maybe (String) } -> { "Type" :: Maybe (String), "Message" :: Maybe (String) }) -> ServiceException
```

Constructs ServiceException's fields from required parameters

#### `Timeout`

``` purescript
newtype Timeout
  = Timeout Int
```

##### Instances
``` purescript
Newtype Timeout _
Generic Timeout _
Show Timeout
Decode Timeout
Encode Timeout
```

#### `UpdateFunctionConfigurationRequest`

``` purescript
newtype UpdateFunctionConfigurationRequest
  = UpdateFunctionConfigurationRequest { "FunctionName" :: FunctionName, "Role" :: Maybe (RoleArn), "Handler" :: Maybe (Handler), "Description" :: Maybe (Description), "Timeout" :: Maybe (Timeout), "MemorySize" :: Maybe (MemorySize) }
```

##### Instances
``` purescript
Newtype UpdateFunctionConfigurationRequest _
Generic UpdateFunctionConfigurationRequest _
Show UpdateFunctionConfigurationRequest
Decode UpdateFunctionConfigurationRequest
Encode UpdateFunctionConfigurationRequest
```

#### `newUpdateFunctionConfigurationRequest`

``` purescript
newUpdateFunctionConfigurationRequest :: FunctionName -> UpdateFunctionConfigurationRequest
```

Constructs UpdateFunctionConfigurationRequest from required parameters

#### `newUpdateFunctionConfigurationRequest'`

``` purescript
newUpdateFunctionConfigurationRequest' :: FunctionName -> ({ "FunctionName" :: FunctionName, "Role" :: Maybe (RoleArn), "Handler" :: Maybe (Handler), "Description" :: Maybe (Description), "Timeout" :: Maybe (Timeout), "MemorySize" :: Maybe (MemorySize) } -> { "FunctionName" :: FunctionName, "Role" :: Maybe (RoleArn), "Handler" :: Maybe (Handler), "Description" :: Maybe (Description), "Timeout" :: Maybe (Timeout), "MemorySize" :: Maybe (MemorySize) }) -> UpdateFunctionConfigurationRequest
```

Constructs UpdateFunctionConfigurationRequest's fields from required parameters

#### `UploadFunctionRequest`

``` purescript
newtype UploadFunctionRequest
  = UploadFunctionRequest { "FunctionName" :: FunctionName, "FunctionZip" :: String, "Runtime" :: Runtime, "Role" :: RoleArn, "Handler" :: Handler, "Mode" :: Mode, "Description" :: Maybe (Description), "Timeout" :: Maybe (Timeout), "MemorySize" :: Maybe (MemorySize) }
```

##### Instances
``` purescript
Newtype UploadFunctionRequest _
Generic UploadFunctionRequest _
Show UploadFunctionRequest
Decode UploadFunctionRequest
Encode UploadFunctionRequest
```

#### `newUploadFunctionRequest`

``` purescript
newUploadFunctionRequest :: FunctionName -> String -> Handler -> Mode -> RoleArn -> Runtime -> UploadFunctionRequest
```

Constructs UploadFunctionRequest from required parameters

#### `newUploadFunctionRequest'`

``` purescript
newUploadFunctionRequest' :: FunctionName -> String -> Handler -> Mode -> RoleArn -> Runtime -> ({ "FunctionName" :: FunctionName, "FunctionZip" :: String, "Runtime" :: Runtime, "Role" :: RoleArn, "Handler" :: Handler, "Mode" :: Mode, "Description" :: Maybe (Description), "Timeout" :: Maybe (Timeout), "MemorySize" :: Maybe (MemorySize) } -> { "FunctionName" :: FunctionName, "FunctionZip" :: String, "Runtime" :: Runtime, "Role" :: RoleArn, "Handler" :: Handler, "Mode" :: Mode, "Description" :: Maybe (Description), "Timeout" :: Maybe (Timeout), "MemorySize" :: Maybe (MemorySize) }) -> UploadFunctionRequest
```

Constructs UploadFunctionRequest's fields from required parameters


