# SCOPE-Jev

## Overview

SCOPE-Jev is a candidate-level verification method for tiny object detection in optical remote sensing imagery. Given a candidate bounding box and its predicted class, it combines local visual evidence with the surrounding scene to estimate whether the specified object is present.

The method groups nearby candidates within a bounded shared context window while preserving coverage of their local views. A shared prefix encodes the neighborhood image and common verification instructions once. Each candidate then receives an independent branch containing its own local image, bounding-box coordinates, and class-specific question.

Each branch produces a yes/no verification probability through a structured decision interface. These probabilities support reranking or filtering existing detections while keeping their bounding boxes and class labels unchanged.

The design combines shared scene computation with candidate-specific visual evidence: neighboring candidates reuse common context while retaining separate inputs and subsequent computation for their individual decisions.

## Dataset: TinyRS-Verify

TinyRS-Verify is a candidate-level semantic verification dataset constructed from RS-STOD optical remote sensing imagery and detection annotations. It covers five object categories: small vehicles, large vehicles, ships, airplanes, and storage tanks.

The dataset organizes candidate boxes, class-specific questions, semantic labels, source and split information, and geometric mappings between local and context views. Each verification question asks whether the specified class is present within the designated candidate box.

TinyRS-Verify supports supervised adaptation and evaluation of candidate verification. Its evaluation protocol distinguishes candidate-level semantic judgments from full-image object detection, where predictions must also satisfy localization and matching criteria.

Dataset documentation and access information: **Coming soon.**

## Code and Models

Coming soon.

## Installation and Usage

Coming soon.

## Paper and Citation

Coming soon.
