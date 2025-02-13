---
title: Dynamsoft Label Recognizer Parameter Reference - Main Page
description: Dynamsoft Label Recognizer  Parameter Reference - Main Page
keywords: parameter reference, parameters, label recognition
needAutoGenerateSidebar: false
permalink: /parameters/reference/index.html
---

# Parameter Reference

## Capture Vision Template

 | Parameter Name                                                               | Description |
 | ---------------------------------------------------------------------------- | ----------- |
 | [`ImageROIProcessingNameArray`]({{ site.dcv_parameters_reference }}capture-vision-template/image-roi-processing-name-array.html) | Defines the collection of image ROI processing object names, used to refer to the `TargetROIDef` objects. |
 | [`ImageSourceName`]({{ site.dcv_parameters_reference }}capture-vision-template/image-source-name.html) | Indicates the input source name, used to refer to the `ImageSource` object. |
 | [`MaxParallelTasks`]({{ site.dcv_parameters_reference }}capture-vision-template/max-parallel-tasks.html) | Defines the maximum number of parallel tasks for the DCV runtime. |
 | [`OutputRawImage`]({{ site.dcv_parameters_reference }}capture-vision-template/output-raw-Image.html) | Indicates whether DCV finally outputs the original input image. |
 | [`SemanticProcessingNameArray`]({{ site.dcv_parameters_reference }}capture-vision-template/semantic-processing-name-array.html) | Represents the collection of semantic-processing object names, used to refer to the `SematicProcessing` objects. |
 | [`Timeout`]({{ site.dcv_parameters_reference }}capture-vision-template/timeout.html) | Defines the maximum amount of time (in milliseconds) that should be spent processing each image or frame. |

## Target ROI Def

 | Parameter Name                                                                        | Description |
 | ------------------------------------------------------------------------------------- | ----------- |
 | [`BaseTargetROIDefName`]({{ site.dcv_parameters_reference }}target-roi-def/base-target-roidef-name.html) | Represents the name of another `TargetROIDef` object to inherit from. |
 | [`Location`]({{ site.dcv_parameters_reference }}target-roi-def/location.html) | Defines the location of the TargetROI with `reference objects` filter conditions and `offset` parameters. |
 | [`PauseFlag`]({{ site.dcv_parameters_reference }}target-roi-def/pause-flag.html) | Indicates that the region results generated by this `TargetROIDef` will not be used by other `TargetROIDef` objects that depend on it to calculate the target regions, unless the user explicitly performs an update operation. |
 | [`TaskSettingNameArray`]({{ site.dcv_parameters_reference }}target-roi-def/task-setting-name-array.html) | Parameter `TaskSettingNameArray` represents the collection of task setting object names, used to refer to the `LabelRecognizerTaskSetting` objects. |

## Label Recognizer Task Setting

 | Parameter Name                                                                                                            | Description |
 | ------------------------------------------------------------------------------------------------------------------------- | ----------- |
 | [`BaseLabelRecognizerTaskSettingName`]({{ site.dcv_parameters_reference }}label-recognizer-task-settings/base-label-recognizer-task-setting-name.html) | Represents the name of another `LabelRecognizerTaskSetting` object to inherit from. |
 | [`DictionaryCorrectionThresholds`]({{ site.dcv_parameters_reference }}label-recognizer-task-settings/dictionary-correction-thresholds.html) | Sets the threshold of dictionary error correction. |
 | [`DictionaryPath`]({{ site.dcv_parameters_reference }}label-recognizer-task-settings/dictionary-path.html) | Sets the path of the dictionary file.|
 | [`StringLengthRange`]({{ site.dcv_parameters_reference }}label-recognizer-task-settings/string-length-range.html) | Sets the range of string lengths for concatenated strings of recognized text lines. |
 | [`StringRegExPattern`]({{ site.dcv_parameters_reference }}label-recognizer-task-settings/string-regex-pattern.html) | Specifies the regular expression pattern for concatenated strings of recognized text lines. |

## TextLine Specification

| Parameter Name                                                                        | Description |
 | ------------------------------------------------------------------------------------- | ----------- |
 | [`ApplicableTextLineNumbers`]({{ site.dcv_parameters_reference }}text-line-specification/applicable-text-line-numbers.html) | Specifies the line numers of the targeting lines which are specified by the `TextLineSpecification` object. |
 | [`BaseTextLineSpecificationName`]({{ site.dcv_parameters_reference }}text-line-specification/base-text-line-specification-name.html) | Represents the name of another `TextLineSpecification` object to inherit from. |
 | [`CharHeightRange`]({{ site.dcv_parameters_reference }}text-line-specification/char-height-range.html) | Defines the range of the character height. |
 | [`CharacterModelName`]({{ site.dcv_parameters_reference }}text-line-specification/character-model-name.html) | Defines the name of the character model. |
 | [`CharacterNormalizationModes`]({{ site.dcv_parameters_reference }}text-line-specification/character-normalization-modes.html) | Defines an array of character normalization mode to implement. The array index represents the priority of the item. The smaller index is, the higher priority is. |
 | [`Text line position parameters`]({{ site.dcv_parameters_reference }}text-line-specification/position.html) | Defines the position of the text lines with the vertices points. |

## Character Model

 | Parameter Name                                                                        | Description |
 | ------------------------------------------------------------------------------------- | ----------- |
 | [`FilterFilePath`]({{ site.dcv_parameters_reference }}character-model/filter-file-path.html) | Defines the full path of the filter file which specifies the characters to be recognized. |

## ImageParameter

 | Parameter Name                                                                                       | Description |
 | ---------------------------------------------------------------------------------------------------- | ----------- |
 | [`BaseImageParameterName`]({{ site.dcv_parameters_reference }}image-parameter/base-image-parameter-name.html) | Represents the name of another `ImageParameter` object to inherit from. |
 | [`BinarizationModes`]({{ site.dcv_parameters_reference }}image-parameter/binarization-modes.html) | Defines the process of binarization |
 | [`ColourChannelUsageType`]({{ site.dcv_parameters_reference }}image-parameter/colour-channel-usage-type.html) | Defines how to use the colour channel from the source image buffer. |
 | [`ColourConversionModes`]({{ site.dcv_parameters_reference }}image-parameter/colour-conversion-modes.html) | Defines how to convert a colour image to a grayscale image. |
 | [`GrayscaleEnhancementModes`]({{ site.dcv_parameters_reference }}image-parameter/grayscale-enhancement-modes.html) | Defines the image processing methods to enhance the quality of the grayscale image. |
 | [`GrayscaleTransformationModes`]({{ site.dcv_parameters_reference }}image-parameter/grayscale-transformation-modes.html) | Defines whether or not to invert the color of the grayscale image. |
 | [`IfEraseTextZone`]({{ site.dcv_parameters_reference }}image-parameter/if-erase-text-zone.html) | Defines whether to erase the detected text zone. |
 | [`RegionPredetectionModes`]({{ site.dcv_parameters_reference }}image-parameter/region-predetection-modes.html) | Defines how to find a region of interest (ROI) within the image or frame. |
 | [`ScaleDownThreshold`]({{ site.dcv_parameters_reference }}image-parameter/scale-down-threshold.html) | Defines the threshold for image shrinking. |
 | [`ScaleUpModes`]({{ site.dcv_parameters_reference }}image-parameter/scale-up-modes.html) | Defines the scale-up process when targets in the image are too small. |
 | [`TextDetectionMode`]({{ site.dcv_parameters_reference }}image-parameter/text-detection-mode.html) | Defines how to detect the text area. |
 | [`TextureDetectionModes`]({{ site.dcv_parameters_reference }}image-parameter/texture-detection-modes.html) | Defines how to detect texture on an image. |

## Image Source Options

 | Parameter Name                                                           | Description |
 | ------------------------------------------------------------------------ | ----------- |
 | [`FileFilter`]({{ site.dcv_parameters_reference }}image-source-options/file-filter.html) | Defines a file name filter string, which determines which files are fetched. |
 | [`PDFReadingMode`]({{ site.dcv_parameters_reference }}image-source-options/pdf-reading-mode.html) | Defines how to handle PDF files. |
 | [`Recursive`]({{ site.dcv_parameters_reference }}image-source-options/recursive.html) | Defines whether to fetch files recursively. |
 | [`Type`]({{ site.dcv_parameters_reference }}image-source-options/type.html) | Defines the type of the ImageSource object, which helps CVR create the correct type of image source. |

## Global Parameter

 | Parameter Name                                                                            | Description |
 | ----------------------------------------------------------------------------------------- | ----------- |
 | [`MaxTotalImageDimension`]({{ site.dcv_parameters_reference }}global-parameter/max-total-image-dimension.html) | Defines the maximum total dimension of the images that read in the memory |

## Shared Parameter

 | Parameter Name                                                                                    | Description |
 | ------------------------------------------------------------------------------------------------- | ----------- |
 | [`DirectoryPath`]({{ site.dcv_parameters_reference }}shared-parameter/directory-path.html) | Defines a path when the library have to read files. |
 | [`MaxThreadsInOneTask`]({{ site.dcv_parameters_reference }}shared-parameter/max-threads-in-one-task.html) | Defines the maximum threads that can be consumed in one task. |
 | [`Name`]({{ site.dcv_parameters_reference }}shared-parameter/name.html) | Represents the name of the top-level objects in Dynamsoft Capture Vision Parameter Template, which serves as its unique identifier. |
 | [`SectionImageParameterArray`]({{ site.dcv_parameters_reference }}shared-parameter/section-image-parameter-array.html) | Defines the image processing algorithms that implemented in the task. |
 | [`StartSection`]({{ site.dcv_parameters_reference }}shared-parameter/start-section.html) | Defines the start section of the algorithm task. |
 | [`TerminateSetting`]({{ site.dcv_parameters_reference }}shared-parameter/terminate-setting.html) | Defines the terminate stages of the task. |