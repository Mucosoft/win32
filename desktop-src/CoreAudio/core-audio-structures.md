---
Description: Core Audio Structures
ms.assetid: 92585cd4-baa9-4f75-816e-b83f5badad37
title: Core Audio Structures
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Core Audio Structures

This section describes the structures that are used by the Core Audio APIs in Windows Vista and later.



| Structure                                                                     | Description                                                                                                                                                         |
|-------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**AUDIO\_VOLUME\_NOTIFICATION\_DATA**](/windows/desktop/api/Endpointvolume/ns-endpointvolume-audio_volume_notification_data)   | Describes a change in the volume level or muting state of an audio endpoint device.                                                                                 |
| [**DIRECTX\_AUDIO\_ACTIVATION\_PARAMS**](/windows/desktop/api/Mmdeviceapi/ns-mmdeviceapi-tagdirectx_audio_activation_params) | Specifies the initialization parameters for a DirectSound stream.                                                                                                   |
| [**KSJACK\_DESCRIPTION**](/windows/desktop/api/Devicetopology/ns-devicetopology-__midl___midl_itf_devicetopology_0000_0000_0009)                             | Retrieved through [**IKsJackDescription::GetJackDescription**](/windows/desktop/api/Devicetopology/nf-devicetopology-iksjackdescription-getjackdescription); describes an audio jack.                                 |
| [**KSJACK\_DESCRIPTION2**](/windows/desktop/api/Devicetopology/ns-devicetopology-_tagksjack_description2)<br/>                | Retrieved through [**IKsJackDescription2::GetJackDescription2**](/windows/desktop/api/Devicetopology/nf-devicetopology-iksjackdescription2-getjackdescription2); describes an audio jack. <br/>                 |
| [**KSJACK\_SINK\_INFORMATION**](/windows/desktop/api/Devicetopology/ns-devicetopology-_tagksjack_sink_information)<br/>       | Retrieved through [**IKsJackSinkInformation::GetJackSinkInformation**](/windows/desktop/api/Devicetopology/nf-devicetopology-iksjacksinkinformation-getjacksinkinformation); describes an audio jack sink.<br/> |
| [**LUID**](/windows/desktop/api/Devicetopology/ns-devicetopology-_luid)<br/>                                               | Stores the video port identifier.<br/>                                                                                                                        |



 

## Related topics

<dl> <dt>

[Programming Reference](programming-reference.md)
</dt> </dl>

 

 



