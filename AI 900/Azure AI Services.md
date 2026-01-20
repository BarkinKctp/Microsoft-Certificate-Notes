## Azure AI Resources

• **Multi-service resource**:  
A resource created in the Azure portal that provides access to multiple Azure AI services with a single key and endpoint. Use the Azure AI services resource when you need several AI services or are exploring AI capabilities. When you use a multi-service resource, all AI services are billed together.

• **Single-service resources**:  
A resource created in the Azure portal that provides access to a single Azure AI service, such as Speech, Vision, or Language. Each service has a unique key and endpoint. These resources are useful when you only need one AI service or want to track costs separately.

To explore the capabilities of a service in the studio, you must first associate the resource with the studio.

---

## Key Concepts and Terminology

• **API (Application Programming Interface)**:  
Enables software components to communicate so one side can be updated without stopping the other.

• **Artificial Intelligence (AI)**:  
Computer programs that respond in ways normally associated with human reasoning, learning, and thought.

• **Azure AI services**:  
A portfolio of AI services that can be incorporated into applications quickly and easily without specialist knowledge. Also refers to the multi-service resource created in the Azure portal.

• **Endpoint**:  
The location of a resource, such as an Azure AI service.

• **Key**:  
A private string used to authenticate a request.

• **Machine learning**:  
The ability for computer programs to learn from large amounts of data through a process called training.

• **Multi-service resource**:  
An AI service resource that provides access to multiple Azure AI services.

• **Single-service resource**:  
A resource that provides access to only one Azure AI service, each with its own key and endpoint.

• **RESTful API**:  
A scalable web API used to access Azure AI services.

---

=========================================================================

## Azure AI Services Overview

• **Azure AI Bot Service** provides a platform for conversational AI, enabling software agents to participate in conversations.

• **Azure AI Translator** is part of Natural Language Processing (NLP) but is not a platform for conversational AI.

• **Azure AI Vision** focuses on image processing capabilities.

• **Azure AI Document Intelligence** extracts information from scanned documents such as forms and invoices.

• **Text translation** and **document translation** are part of the Translator service.

• **Language identification**, **speaker recognition**, and **voice assistants** are components of the Azure AI Speech service.

• **Custom Translator with dictionaries** can be used when there are not enough parallel sentences (less than 10,000). This approach results in faster training and uses baseline models combined with provided dictionaries.

• **Azure AI Speech** provides speech-to-text and text-to-speech through recognition and synthesis. It supports prebuilt and custom models for:
  - Audio transcription
  - Speaker identification
  - Custom voice creation
  - Speech translation

• **Translating speech to text** is an example of speech translation and uses the Azure AI Speech service as part of Azure AI Services.
