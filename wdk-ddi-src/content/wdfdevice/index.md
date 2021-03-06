---
UID: NA:wdfdevice
ms.assetid: 24b2e402-56ef-3f36-b4f0-426a9d758500
ms.date: 05/09/18
ms.keywords: 
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: portal
product:
-	Windows
tech.root: wdf
---

# Wdfdevice.h header


## -description


This header is used by wdf. For more information, see:

- [Windows Driver Framework](../_wdf/index.md)
- [wdffdo.h header](../wdffdo/index.md)
- [wdfpdo.h header](../wdfpdo/index.md)

This topic orders the Windows Driver Frameworks (WDF) device object reference by category.

The categories on this page are:

-   [General Framework Device Object Event Callback Functions](#general-framework-device-object-event-callback-functions)
-   [General Framework Device Object Initialization Methods](#general-framework-device-object-initialization-methods)
-   [General Framework Device Object Methods](#general-framework-device-object-methods)
-   [General Framework Device Object Structures and Enumerations](#general-framework-device-object-structures-and-enumerations)
-   [Initialization Functions for Device Object Structures](#initialization-functions-for-device-object-structures)

## General Framework Device Object Event Callback Functions

-   [*EvtDeviceArmWakeFromS0*](https://msdn.microsoft.com/library/windows/hardware/ff540843)
-   [*EvtDeviceArmWakeFromSx*](https://msdn.microsoft.com/library/windows/hardware/ff540844)
-   [*EvtDeviceArmWakeFromSxWithReason*](https://msdn.microsoft.com/library/windows/hardware/ff540846)
-   [*EvtDeviceD0Entry*](https://msdn.microsoft.com/library/windows/hardware/ff540848)
-   [*EvtDeviceD0EntryPostInterruptsEnabled*](https://msdn.microsoft.com/library/windows/hardware/ff540853)
-   [*EvtDeviceD0Exit*](https://msdn.microsoft.com/library/windows/hardware/ff540855)
-   [*EvtDeviceD0ExitPreInterruptsDisabled*](https://msdn.microsoft.com/library/windows/hardware/ff540856)
-   [*EvtDeviceDisarmWakeFromS0*](https://msdn.microsoft.com/library/windows/hardware/ff540860)
-   [*EvtDeviceDisarmWakeFromSx*](https://msdn.microsoft.com/library/windows/hardware/ff540862)
-   [*EvtDeviceFileCreate*](https://msdn.microsoft.com/library/windows/hardware/ff540868)
-   [*EvtDevicePnpStateChange*](https://msdn.microsoft.com/library/windows/hardware/ff540874)
-   [*EvtDevicePowerPolicyStateChange*](https://msdn.microsoft.com/library/windows/hardware/ff540876)
-   [*EvtDevicePowerStateChange*](https://msdn.microsoft.com/library/windows/hardware/ff540878)
-   [*EvtDevicePrepareHardware*](https://msdn.microsoft.com/library/windows/hardware/ff540880)
-   [*EvtDeviceQueryRemove*](https://msdn.microsoft.com/library/windows/hardware/ff540883)
-   [*EvtDeviceQueryStop*](https://msdn.microsoft.com/library/windows/hardware/ff540885)
-   [*EvtDeviceRelationsQuery*](https://msdn.microsoft.com/library/windows/hardware/ff540886)
-   [*EvtDeviceReleaseHardware*](https://msdn.microsoft.com/library/windows/hardware/ff540890)
-   [*EvtDeviceSelfManagedIoCleanup*](https://msdn.microsoft.com/library/windows/hardware/ff540898)
-   [*EvtDeviceSelfManagedIoFlush*](https://msdn.microsoft.com/library/windows/hardware/ff540901)
-   [*EvtDeviceSelfManagedIoInit*](https://msdn.microsoft.com/library/windows/hardware/ff540902)
-   [*EvtDeviceSelfManagedIoRestart*](https://msdn.microsoft.com/library/windows/hardware/ff540905)
-   [*EvtDeviceSelfManagedIoSuspend*](https://msdn.microsoft.com/library/windows/hardware/ff540907)
-   [*EvtDeviceSurpriseRemoval*](https://msdn.microsoft.com/library/windows/hardware/ff540913)
-   [*EvtDeviceUsageNotification*](https://msdn.microsoft.com/library/windows/hardware/ff540915)
-   [*EvtDeviceUsageNotificationEx*](https://msdn.microsoft.com/library/windows/hardware/hh406365)
-   [*EvtDeviceWakeFromS0Triggered*](https://msdn.microsoft.com/library/windows/hardware/ff540919)
-   [*EvtDeviceWakeFromSxTriggered*](https://msdn.microsoft.com/library/windows/hardware/ff540923)
-   [*EvtDeviceWdmIrpDispatch*](https://msdn.microsoft.com/library/windows/hardware/hh406404)
-   [*EvtDeviceWdmIrpPreprocess*](https://msdn.microsoft.com/library/windows/hardware/ff540925)
-   [*EvtDeviceWdmPostPoFxRegisterDevice*](https://msdn.microsoft.com/library/windows/hardware/hh406408)
-   [*EvtDeviceWdmPrePoFxUnregisterDevice*](https://msdn.microsoft.com/library/windows/hardware/hh406411)
-   [*EvtFileCleanup*](https://msdn.microsoft.com/library/windows/hardware/ff541700)
-   [*EvtFileClose*](https://msdn.microsoft.com/library/windows/hardware/ff541702)
-   [*EvtIoInCallerContext*](https://msdn.microsoft.com/library/windows/hardware/ff541764)

## General Framework Device Object Initialization Methods

-   [**WdfDeviceInitAssignName**](https://msdn.microsoft.com/library/windows/hardware/ff546029)
-   [**WdfDeviceInitAssignSDDLString**](https://msdn.microsoft.com/library/windows/hardware/ff546035)
-   [**WdfDeviceInitAssignWdmIrpPreprocessCallback**](https://msdn.microsoft.com/library/windows/hardware/ff546043)
-   [**WdfDeviceInitFree**](https://msdn.microsoft.com/library/windows/hardware/ff546050)
-   [**WdfDeviceInitRegisterPnpStateChangeCallback**](https://msdn.microsoft.com/library/windows/hardware/ff546057)
-   [**WdfDeviceInitRegisterPowerPolicyStateChangeCallback**](https://msdn.microsoft.com/library/windows/hardware/ff546066)
-   [**WdfDeviceInitRegisterPowerStateChangeCallback**](https://msdn.microsoft.com/library/windows/hardware/ff546071)
-   [**WdfDeviceInitSetCharacteristics**](https://msdn.microsoft.com/library/windows/hardware/ff546074)
-   [**WdfDeviceInitSetDeviceClass**](https://msdn.microsoft.com/library/windows/hardware/ff546084)
-   [**WdfDeviceInitSetDeviceType**](https://msdn.microsoft.com/library/windows/hardware/ff546090)
-   [**WdfDeviceInitSetExclusive**](https://msdn.microsoft.com/library/windows/hardware/ff546097)
-   [**WdfDeviceInitSetFileObjectConfig**](https://msdn.microsoft.com/library/windows/hardware/ff546107)
-   [**WdfDeviceInitSetIoInCallerContextCallback**](https://msdn.microsoft.com/library/windows/hardware/ff546119)
-   [**WdfDeviceInitSetIoType**](https://msdn.microsoft.com/library/windows/hardware/ff546128)
-   [**WdfDeviceInitSetIoTypeEx**](https://msdn.microsoft.com/library/windows/hardware/dn265604)
-   [**WdfDeviceInitSetPnpPowerEventCallbacks**](https://msdn.microsoft.com/library/windows/hardware/ff546135)
-   [**WdfDeviceInitSetPowerInrush**](https://msdn.microsoft.com/library/windows/hardware/ff546142)
-   [**WdfDeviceInitSetPowerNotPageable**](https://msdn.microsoft.com/library/windows/hardware/ff546147)
-   [**WdfDeviceInitSetPowerPageable**](https://msdn.microsoft.com/library/windows/hardware/ff546766)
-   [**WdfDeviceInitSetPowerPolicyEventCallbacks**](https://msdn.microsoft.com/library/windows/hardware/ff546774)
-   [**WdfDeviceInitSetPowerPolicyOwnership**](https://msdn.microsoft.com/library/windows/hardware/ff546776)
-   [**WdfDeviceInitSetReleaseHardwareOrderOnFailure**](https://msdn.microsoft.com/library/windows/hardware/hh706196)
-   [**WdfDeviceInitSetRemoveLockOptions**](https://msdn.microsoft.com/library/windows/hardware/hh451095)
-   [**WdfDeviceInitSetRequestAttributes**](https://msdn.microsoft.com/library/windows/hardware/ff546786)

## General Framework Device Object Methods

-   [**WdfDeviceAddDependentUsageDeviceObject**](https://msdn.microsoft.com/library/windows/hardware/ff545864)
-   [**WdfDeviceAddRemovalRelationsPhysicalDevice**](https://msdn.microsoft.com/library/windows/hardware/ff545875)
-   [**WdfDeviceAllocAndQueryInterfaceProperty**](https://msdn.microsoft.com/library/windows/hardware/dn265598)
-   [**WdfDeviceAllocAndQueryProperty**](https://msdn.microsoft.com/library/windows/hardware/ff545882)
-   [**WdfDeviceAllocAndQueryPropertyEx**](https://msdn.microsoft.com/library/windows/hardware/dn265599)
-   [**WdfDeviceAssignInterfaceProperty**](https://msdn.microsoft.com/library/windows/hardware/dn265600)
-   [**WdfDeviceAssignMofResourceName**](https://msdn.microsoft.com/library/windows/hardware/ff545897)
-   [**WdfDeviceAssignProperty**](https://msdn.microsoft.com/library/windows/hardware/dn265601)
-   [**WdfDeviceAssignS0IdleSettings**](https://msdn.microsoft.com/library/windows/hardware/ff545903)
-   [**WdfDeviceAssignSxWakeSettings**](https://msdn.microsoft.com/library/windows/hardware/ff545909)
-   [**WdfDeviceClearRemovalRelationsDevices**](https://msdn.microsoft.com/library/windows/hardware/ff545914)
-   [**WdfDeviceConfigureRequestDispatching**](https://msdn.microsoft.com/library/windows/hardware/ff545920)
-   [**WdfDeviceConfigureWdmIrpDispatchCallback**](https://msdn.microsoft.com/library/windows/hardware/hh451093)
-   [**WdfDeviceCreate**](https://msdn.microsoft.com/library/windows/hardware/ff545926)
-   [**WdfDeviceCreateDeviceInterface**](https://msdn.microsoft.com/library/windows/hardware/ff545935)
-   [**WdfDeviceCreateSymbolicLink**](https://msdn.microsoft.com/library/windows/hardware/ff545939)
-   [**WdfDeviceEnqueueRequest**](https://msdn.microsoft.com/library/windows/hardware/ff545945)
-   [**WdfDeviceGetAlignmentRequirement**](https://msdn.microsoft.com/library/windows/hardware/ff545953)
-   [**WdfDeviceGetCharacteristics**](https://msdn.microsoft.com/library/windows/hardware/ff545960)
-   [**WdfDeviceGetDefaultQueue**](https://msdn.microsoft.com/library/windows/hardware/ff545965)
-   [**WdfDeviceGetDevicePnpState**](https://msdn.microsoft.com/library/windows/hardware/ff545969)
-   [**WdfDeviceGetDevicePowerPolicyState**](https://msdn.microsoft.com/library/windows/hardware/ff545974)
-   [**WdfDeviceGetDevicePowerState**](https://msdn.microsoft.com/library/windows/hardware/ff545985)
-   [**WdfDeviceGetDeviceStackIoType**](https://msdn.microsoft.com/library/windows/hardware/dn265602)
-   [**WdfDeviceGetDeviceState**](https://msdn.microsoft.com/library/windows/hardware/ff545994)
-   [**WdfDeviceGetDriver**](https://msdn.microsoft.com/library/windows/hardware/ff545998)
-   [**WdfDeviceGetFileObject**](https://msdn.microsoft.com/library/windows/hardware/ff546007)
-   [**WdfDeviceGetHardwareRegisterMappedAddress**](https://msdn.microsoft.com/library/windows/hardware/dn265603)
-   [**WdfDeviceGetIoTarget**](https://msdn.microsoft.com/library/windows/hardware/ff546017)
-   [**WdfDeviceGetSystemPowerAction**](https://msdn.microsoft.com/library/windows/hardware/ff546022)
-   [**WdfDeviceIndicateWakeStatus**](https://msdn.microsoft.com/library/windows/hardware/ff546025)
-   [**WdfDeviceMapIoSpace**](https://msdn.microsoft.com/library/windows/hardware/dn265605)
-   [**WdfDeviceMiniportCreate**](https://msdn.microsoft.com/library/windows/hardware/ff546802)
-   [**WdfDeviceOpenDevicemapKey**](https://msdn.microsoft.com/library/windows/hardware/dn932458)
-   [**WdfDeviceOpenRegistryKey**](https://msdn.microsoft.com/library/windows/hardware/ff546804)
-   [**WdfDevicePostEvent**](https://msdn.microsoft.com/library/windows/hardware/dn265606)
-   [**WdfDeviceQueryInterfaceProperty**](https://msdn.microsoft.com/library/windows/hardware/dn265607)
-   [**WdfDeviceQueryProperty**](https://msdn.microsoft.com/library/windows/hardware/ff546820)
-   [**WdfDeviceQueryPropertyEx**](https://msdn.microsoft.com/library/windows/hardware/dn265608)
-   [**WdfDeviceReadFromHardware**](https://msdn.microsoft.com/library/windows/hardware/dn265609)
-   [**WdfDeviceRemoveDependentUsageDeviceObject**](https://msdn.microsoft.com/library/windows/hardware/ff546829)
-   [**WdfDeviceRemoveRemovalRelationsPhysicalDevice**](https://msdn.microsoft.com/library/windows/hardware/ff546834)
-   [**WdfDeviceResumeIdle**](https://msdn.microsoft.com/library/windows/hardware/ff546838)
-   [**WdfDeviceResumeIdleWithTag**](https://msdn.microsoft.com/library/windows/hardware/dn932459)
-   [**WdfDeviceRetrieveDeviceInterfaceString**](https://msdn.microsoft.com/library/windows/hardware/ff546842)
-   [**WdfDeviceRetrieveDeviceName**](https://msdn.microsoft.com/library/windows/hardware/ff546853)
-   [**WdfDeviceSetAlignmentRequirement**](https://msdn.microsoft.com/library/windows/hardware/ff546861)
-   [**WdfDeviceSetBusInformationForChildren**](https://msdn.microsoft.com/library/windows/hardware/ff546868)
-   [**WdfDeviceSetCharacteristics**](https://msdn.microsoft.com/library/windows/hardware/ff546872)
-   [**WdfDeviceSetDeviceInterfaceState**](https://msdn.microsoft.com/library/windows/hardware/ff546878)
-   [**WdfDeviceSetDeviceState**](https://msdn.microsoft.com/library/windows/hardware/ff546884)
-   [**WdfDeviceSetFailed**](https://msdn.microsoft.com/library/windows/hardware/ff546890)
-   [**WdfDeviceSetPnpCapabilities**](https://msdn.microsoft.com/library/windows/hardware/ff546898)
-   [**WdfDeviceSetPowerCapabilities**](https://msdn.microsoft.com/library/windows/hardware/ff546901)
-   [**WdfDeviceSetSpecialFileSupport**](https://msdn.microsoft.com/library/windows/hardware/ff546903)
-   [**WdfDeviceSetStaticStopRemove**](https://msdn.microsoft.com/library/windows/hardware/ff546915)
-   [**WdfDeviceStopIdle**](https://msdn.microsoft.com/library/windows/hardware/ff546921)
-   [**WdfDeviceStopIdleWithTag**](https://msdn.microsoft.com/library/windows/hardware/dn932460)
-   [**WdfDeviceUnmapIoSpace**](https://msdn.microsoft.com/library/windows/hardware/dn265610)
-   [**WdfDeviceWdmAssignPowerFrameworkSettings**](https://msdn.microsoft.com/library/windows/hardware/hh451097)
-   [**WdfDeviceWdmDispatchIrp**](https://msdn.microsoft.com/library/windows/hardware/hh451100)
-   [**WdfDeviceWdmDispatchIrpToIoQueue**](https://msdn.microsoft.com/library/windows/hardware/hh451105)
-   [**WdfDeviceWdmDispatchPreprocessedIrp**](https://msdn.microsoft.com/library/windows/hardware/ff546927)
-   [**WdfDeviceWdmGetAttachedDevice**](https://msdn.microsoft.com/library/windows/hardware/ff546934)
-   [**WdfDeviceWdmGetDeviceObject**](https://msdn.microsoft.com/library/windows/hardware/ff546942)
-   [**WdfDeviceWdmGetPhysicalDevice**](https://msdn.microsoft.com/library/windows/hardware/ff546946)
-   [**WdfDeviceWriteToHardware**](https://msdn.microsoft.com/library/windows/hardware/dn265611)
-   [**WdfDevStateIsNP**](https://msdn.microsoft.com/library/windows/hardware/ff546958)
-   [**WdfDevStateNormalize**](https://msdn.microsoft.com/library/windows/hardware/ff546966)
-   [**WdfWdmDeviceGetWdfDeviceHandle**](https://msdn.microsoft.com/library/windows/hardware/ff551175)

## General Framework Device Object Structures and Enumerations

-   [**WDF_DEVICE_FAILED_ACTION**](https://msdn.microsoft.com/library/windows/hardware/ff551253)
-   [**WDF_DEVICE_INTERFACE_PROPERTY_DATA**](https://msdn.microsoft.com/library/windows/hardware/dn265629)
-   [**WDF_DEVICE_IO_TYPE**](https://msdn.microsoft.com/library/windows/hardware/ff551255)
-   [**WDF_DEVICE_PNP_CAPABILITIES**](https://msdn.microsoft.com/library/windows/hardware/ff551257)
-   [**WDF_DEVICE_PNP_NOTIFICATION_DATA**](https://msdn.microsoft.com/library/windows/hardware/ff551260)
-   [**WDF_DEVICE_PNP_STATE**](https://msdn.microsoft.com/library/windows/hardware/ff551262)
-   [**WDF_DEVICE_POWER_CAPABILITIES**](https://msdn.microsoft.com/library/windows/hardware/ff551264)
-   [**WDF_DEVICE_POWER_NOTIFICATION_DATA**](https://msdn.microsoft.com/library/windows/hardware/ff551268)
-   [**WDF_DEVICE_POWER_POLICY_IDLE_SETTINGS**](https://msdn.microsoft.com/library/windows/hardware/ff551270)
-   [**WDF_DEVICE_POWER_POLICY_NOTIFICATION_DATA**](https://msdn.microsoft.com/library/windows/hardware/ff551273)
-   [**WDF_DEVICE_POWER_POLICY_STATE**](https://msdn.microsoft.com/library/windows/hardware/ff551275)
-   [**WDF_DEVICE_POWER_POLICY_WAKE_SETTINGS**](https://msdn.microsoft.com/library/windows/hardware/ff551277)
-   [**WDF_DEVICE_POWER_STATE**](https://msdn.microsoft.com/library/windows/hardware/ff551280)
-   [**WDF_DEVICE_PROPERTY_DATA**](https://msdn.microsoft.com/library/windows/hardware/dn265632)
-   [**WDF_DEVICE_STATE**](https://msdn.microsoft.com/library/windows/hardware/ff551284)
-   [**WDF_DISPATCH_IRP_TO_IO_QUEUE_FLAGS**](https://msdn.microsoft.com/library/windows/hardware/hh439503)
-   [**WDF_EVENT_TYPE**](https://msdn.microsoft.com/library/windows/hardware/dn265637)
-   [**WDF_FILEOBJECT_CONFIG**](https://msdn.microsoft.com/library/windows/hardware/ff551319)
-   [**WDF_IO_TYPE_CONFIG**](https://msdn.microsoft.com/library/windows/hardware/dn265642)
-   [**WDF_PNPPOWER_EVENT_CALLBACKS**](https://msdn.microsoft.com/library/windows/hardware/ff552416)
-   [**WDF_POWER_DEVICE_STATE**](https://msdn.microsoft.com/library/windows/hardware/ff552421)
-   [**WDF_POWER_FRAMEWORK_SETTINGS**](https://msdn.microsoft.com/library/windows/hardware/hh406489)
-   [**WDF_POWER_POLICY_EVENT_CALLBACKS**](https://msdn.microsoft.com/library/windows/hardware/ff552424)
-   [**WDF_POWER_POLICY_IDLE_TIMEOUT_CONSTANTS**](https://msdn.microsoft.com/library/windows/hardware/mt845640)
-   [**WDF_POWER_POLICY_IDLE_TIMEOUT_TYPE**](https://msdn.microsoft.com/library/windows/hardware/hh706247)
-   [**WDF_POWER_POLICY_S0_IDLE_CAPABILITIES**](https://msdn.microsoft.com/library/windows/hardware/ff552429)
-   [**WDF_POWER_POLICY_S0_IDLE_USER_CONTROL**](https://msdn.microsoft.com/library/windows/hardware/ff552432)
-   [**WDF_POWER_POLICY_SX_WAKE_USER_CONTROL**](https://msdn.microsoft.com/library/windows/hardware/ff552436)
-   [**WDF_RELEASE_HARDWARE_ORDER_ON_FAILURE**](https://msdn.microsoft.com/library/windows/hardware/hh706249)
-   [**WDF_REMOVE_LOCK_OPTIONS**](https://msdn.microsoft.com/library/windows/hardware/hh406495)
-   [**WDF_REMOVE_LOCK_OPTIONS_FLAGS**](https://msdn.microsoft.com/library/windows/hardware/hh406498)
-   [**WDF_SPECIAL_FILE_TYPE**](https://msdn.microsoft.com/library/windows/hardware/ff552509)
-   [**WDF_STATE_NOTIFICATION_TYPE**](https://msdn.microsoft.com/library/windows/hardware/ff552513)
-   [WDFDEVICE_INIT](https://msdn.microsoft.com/library/windows/hardware/ff546951)

## Initialization Functions for Device Object Structures

-   [**WDF_DEVICE_INTERFACE_PROPERTY_DATA_INIT**](https://msdn.microsoft.com/library/windows/hardware/dn265630)
-   [**WDF_DEVICE_PNP_CAPABILITIES_INIT**](https://msdn.microsoft.com/library/windows/hardware/ff551259)
-   [**WDF_DEVICE_POWER_CAPABILITIES_INIT**](https://msdn.microsoft.com/library/windows/hardware/ff551265)
-   [**WDF_DEVICE_POWER_POLICY_IDLE_SETTINGS_INIT**](https://msdn.microsoft.com/library/windows/hardware/ff551271)
-   [**WDF_DEVICE_POWER_POLICY_WAKE_SETTINGS_INIT**](https://msdn.microsoft.com/library/windows/hardware/ff551279)
-   [**WDF_DEVICE_PROPERTY_DATA_INIT**](https://msdn.microsoft.com/library/windows/hardware/dn265633)
-   [**WDF_DEVICE_STATE_INIT**](https://msdn.microsoft.com/library/windows/hardware/ff551286)
-   [**WDF_FILEOBJECT_CONFIG_INIT**](https://msdn.microsoft.com/library/windows/hardware/ff551321)
-   [**WDF_IO_TYPE_CONFIG_INIT**](https://msdn.microsoft.com/library/windows/hardware/dn265643)
-   [**WDF_PNPPOWER_EVENT_CALLBACKS_INIT**](https://msdn.microsoft.com/library/windows/hardware/ff552418)
-   [**WDF_POWER_FRAMEWORK_SETTINGS_INIT**](https://msdn.microsoft.com/library/windows/hardware/hh406492)
-   [**WDF_POWER_POLICY_EVENT_CALLBACKS_INIT**](https://msdn.microsoft.com/library/windows/hardware/ff552426)
-   [**WDF_REMOVE_LOCK_OPTIONS_INIT**](https://msdn.microsoft.com/library/windows/hardware/hh406501)
