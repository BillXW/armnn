#
# Copyright © 2017 Arm Ltd. All rights reserved.
# SPDX-License-Identifier: MIT
#

list(APPEND armnnClBackendWorkloads_sources
    ClActivationWorkload.cpp
    ClActivationWorkload.hpp
    ClAdditionWorkload.cpp
    ClAdditionWorkload.hpp
    ClBatchNormalizationFloatWorkload.cpp
    ClBatchNormalizationFloatWorkload.hpp
    ClConstantWorkload.cpp
    ClConstantWorkload.hpp
    ClConvertFp16ToFp32Workload.cpp
    ClConvertFp16ToFp32Workload.hpp
    ClConvertFp32ToFp16Workload.cpp
    ClConvertFp32ToFp16Workload.hpp
    ClConvolution2dWorkload.cpp
    ClConvolution2dWorkload.hpp
    ClDepthwiseConvolutionWorkload.cpp
    ClDepthwiseConvolutionWorkload.hpp
    ClDivisionFloatWorkload.cpp
    ClDivisionFloatWorkload.hpp
    ClFloorFloatWorkload.cpp
    ClFloorFloatWorkload.hpp
    ClFullyConnectedWorkload.cpp
    ClFullyConnectedWorkload.hpp
    ClL2NormalizationFloatWorkload.cpp
    ClL2NormalizationFloatWorkload.hpp
    ClLstmFloatWorkload.cpp
    ClLstmFloatWorkload.hpp
    ClMeanWorkload.cpp
    ClMeanWorkload.hpp
    ClMergerWorkload.cpp
    ClMergerWorkload.hpp
    ClMultiplicationWorkload.cpp
    ClMultiplicationWorkload.hpp
    ClNormalizationFloatWorkload.cpp
    ClNormalizationFloatWorkload.hpp
    ClPadWorkload.cpp
    ClPadWorkload.hpp
    ClPermuteWorkload.cpp
    ClPermuteWorkload.hpp
    ClPooling2dWorkload.cpp
    ClPooling2dWorkload.hpp
    ClReshapeWorkload.cpp
    ClReshapeWorkload.hpp
    ClResizeBilinearFloatWorkload.cpp
    ClResizeBilinearFloatWorkload.hpp
    ClSoftmaxBaseWorkload.cpp
    ClSoftmaxBaseWorkload.hpp
    ClSoftmaxFloatWorkload.cpp
    ClSoftmaxFloatWorkload.hpp
    ClSoftmaxUint8Workload.cpp
    ClSoftmaxUint8Workload.hpp
    ClSplitterWorkload.hpp
    ClSubtractionWorkload.cpp
    ClSubtractionWorkload.hpp
    ClWorkloads.hpp
    ClWorkloadUtils.hpp
)

add_library(armnnClBackendWorkloads OBJECT ${armnnClBackendWorkloads_sources})
target_include_directories(armnnClBackendWorkloads PRIVATE ${PROJECT_SOURCE_DIR}/src/armnn)
target_include_directories(armnnClBackendWorkloads PRIVATE ${PROJECT_SOURCE_DIR}/src/armnnUtils)
target_include_directories(armnnClBackendWorkloads PRIVATE ${PROJECT_SOURCE_DIR}/src/backends)
