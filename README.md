English Description

DicomView PRO is an advanced, modular DICOM viewer and medical imaging workstation developed by Ivan Kiranchuk (KirivSoft). It is designed for research, clinical testing, and educational use, offering a comprehensive suite of tools for visualizing, processing, and analyzing medical imaging data (CT, MR, XA/XRF, etc.) without requiring a certified PACS infrastructure.

Key Features

    Multi‑plane visualization: 2D axial/coronal/sagittal views, high‑fidelity MPR (multi‑planar reconstruction) with anisotropic spacing compensation, MIP/MinIP/Average projections, and cine/angio playback for multi‑frame DICOM.

    Advanced 3D rendering: VTK‑based volume and surface rendering with cinematic presets, interactive clipping (box, plane, scalpel), 3D ruler, and real‑time transfer function adjustments (HU thresholds, opacity).

    Clinical protocols: Deterministic, CPU‑only algorithms for hemorrhage, trauma, ischemia, tumor, abscess, stone, and vascular lesion detection—generating masks, volume measurements, and structured reports (no AI required).

    AI integration (optional): Support for ONNX runtime (MobileSAM segmentation, denoising, super‑resolution) and TotalSegmentator organ segmentation via external Python runtime; all AI modules are optional and safe‑fallback.

    DICOM connectivity: Built‑in clients for PACS (C‑ECHO, C‑FIND, C‑STORE), Orthanc REST API, and DICOMweb (QIDO‑WADO‑STOW), with local DICOMDIR/USB/CD export.

    Reporting & export: PDF/DOCX reports (with fallback to TXT), JSON structured reports, screenshot capture, 3D mesh export (STL/OBJ/PLY/GLB), and anonymized ZIP archives.

    Modular architecture: Event‑bus, task manager, and module supervisor allow heavy operations (DICOM scanning, segmentation, report generation) to run in background threads or separate processes, keeping the UI responsive.

    Cross‑platform: Built with Python 3.11+, PySide6 (Qt), VTK, and pydicom; packaged as a portable folder or Windows installer.

Technology Stack

    GUI: PySide6 (Qt6) with custom dark/light themes.

    3D rendering: VTK (volume ray casting, surface extraction, clipping).

    Image processing: NumPy, SciPy, SimpleITK, OpenCV (optional), Pillow.

    DICOM: pydicom, python‑gdcm, pylibjpeg plugins (JPEG/JPEG2000/RLE).

    AI/ML: onnxruntime, TotalSegmentator (optional), MobileSAM.

    Packaging: PyInstaller, InnoSetup.

Status & Disclaimer

DicomView PRO is a research and testing prototype, not a certified medical device. All clinical measurements, segmentation, and AI outputs are for visual assistance only—final diagnosis must be made by a qualified clinician on original DICOM data. The software is actively developed, with regular updates (versions v7.x to v9.5.2) focusing on stability, performance, and new clinical modules.

Target Audience

Medical researchers, radiologists in training, PACS administrators, and developers who need a flexible, extensible DICOM viewer for non‑diagnostic workflows, algorithm testing, and educational demonstrations.
Український опис

DicomView PRO — це сучасний модульний DICOM-переглядач та медична робоча станція, розроблена Іваном Кіранчуком (KirivSoft). Програма призначена для дослідницьких, клінічних тестових та навчальних цілей, надаючи широкий набір інструментів для візуалізації, обробки та аналізу медичних зображень (КТ, МР, XA/XRF тощо) без потреби у сертифікованій PACS-інфраструктурі.

Ключові можливості

    Багатоплощинна візуалізація: 2D аксіальні/корональні/сагітальні зрізи, високоякісний MPR (мультиплощинна реконструкція) з компенсацією анізотропного інтервалу, MIP/MinIP/AvgIP проекції, відтворення cine/ангіо для багатокадрових DICOM.

    Розширена 3D-візуалізація: об'ємний та поверхневий рендеринг на основі VTK з кінематографічними пресетами, інтерактивне відсікання (бокс, площина, скальпель), 3D-лінійка та налаштування передавальної функції в реальному часі (HU-пороги, прозорість).

    Клінічні протоколи: детерміновані алгоритми на основі HU та морфології (без ШІ) для виявлення крововиливів, травм, ішемії, пухлин, абсцесів, каменів та судинних уражень — формування масок, вимірювання об'ємів та структуровані звіти.

    Інтеграція ШІ (опціонально): підтримка ONNX Runtime (сегментація MobileSAM, зменшення шуму, суперроздільність) та TotalSegmentator для сегментації органів через зовнішній Python-рантайм; всі ШІ-модулі опціональні та мають безпечний fallback.

    DICOM-з'єднання: вбудовані клієнти для PACS (C-ECHO, C-FIND, C-STORE), Orthanc REST API та DICOMweb (QIDO-WADO-STOW) з експортом на USB/CD/DICOMDIR.

    Звітність та експорт: PDF/DOCX звіти (з fallback на TXT), JSON-звіти, знімки екрану, експорт 3D-мешів (STL/OBJ/PLY/GLB) та анонімізовані ZIP-архіви.

    Модульна архітектура: шина подій, менеджер завдань та супервізор модулів дозволяють виконувати важкі операції (сканування DICOM, сегментація, генерація звітів) у фонових потоках або окремих процесах, зберігаючи чуйність інтерфейсу.

    Крос-платформеність: написано на Python 3.11+ з використанням PySide6 (Qt), VTK та pydicom; пакується як портативна папка або інсталятор для Windows.

Технологічний стек

    GUI: PySide6 (Qt6) з темною/світлою темами.

    3D-рендеринг: VTK (об'ємний рей-кастинг, екстракція поверхонь, відсікання).

    Обробка зображень: NumPy, SciPy, SimpleITK, OpenCV (опціонально), Pillow.

    DICOM: pydicom, python‑gdcm, pylibjpeg (JPEG/JPEG2000/RLE).

    ШІ/ML: onnxruntime, TotalSegmentator (опціонально), MobileSAM.

    Пакування: PyInstaller, InnoSetup.

Статус та застереження

DicomView PRO є дослідницьким та тестовим прототипом, а не сертифікованим медичним виробом. Всі клінічні вимірювання, сегментація та результати ШІ призначені лише для візуальної допомоги — остаточний діагноз повинен ставити кваліфікований лікар на основі оригінальних DICOM-даних. Програма активно розвивається, регулярно оновлюється (версії v7.x – v9.5.2) з акцентом на стабільність, продуктивність та нові клінічні модулі.

Цільова аудиторія

Медичні дослідники, лікарі-стажисти, адміністратори PACS та розробники, які потребують гнучкого, розширюваного DICOM-переглядача для недіагностичних робочих процесів, тестування алгоритмів та навчальних демонстрацій.
