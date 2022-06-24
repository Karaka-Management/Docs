# Development Risk Control Matrix

| No.  | R                 | Category                       | Risk Event                                                   | L    | C    | O                 | Mitigation Type              | Mitigation Strategy                                          | L*   | C*   | Changes | Comments                                                     | ES   | EY   |
| ---- | ----------------- | ------------------------------ | ------------------------------------------------------------ | ---- | ---- | ----------------- | ---------------------------- | ------------------------------------------------------------ | ---- | ---- | ------- | ------------------------------------------------------------ | ---- | ---- |
| 1    | CTO               | Operational Risk (Development) | Unauthorized source code and development asset access.       | 1    | 1    | Many times a day  | Preventing (System & Manual) | Only authorized people gain access to confidential source code and development assets. | 1    | 1    |         | Not all source code and development assets are considered confidential and may be publicly accessible. The confidential aspects are determined by the CTO. | yes  | yes  |
| 2    | CTO               | Operational Risk (Development) | Undefined terms of intellectual property for code contributions. | 1    | 3    | Many times a day  | Preventing (Manual)          | The terms of intellectual property for all contributions are well defined. | 1    | 1    |         |                                                              | yes  | yes  |
| 3    | CTO/Code reviewer | Operational Risk (Development) | Inconsistent code styles (which increases frictions between developers) | 5    | 1    | Many times a day  | Preventing (System & Manual) | Code styles are automatically tested with code style checkers. | 2    | 1    |         | Not all code style options can be reasonably checked and defined. In some cases it's also possible to have false positive code style violations for edge cases. Manual checks during the code review by the responsible person may lead to additional code style changes or ignoring some code style "violations" if deemed reasonable. | yes  | yes  |
| 4    | CTO/Code reviewer | Operational Risk (Development) | Faulty code due to code changes, additions, removal.         | 5    | 4    | Many times  a day | Preventing (System & Manual) | Static code analysis tools and written tests for automatic tests. Additionally, manual tests can be performed in a demo environment with self generated dummy data. | 2    | 1    |         |                                                              |      |      |
