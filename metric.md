```
[metrics-clojure "2.7.0"]

(def ^:private booking-created-meter (mk-meter "bookings" "created"))

(defn booking-created! []
 (mark! booking-created-meter))
```

Whenever event happens:
Call → `(booking-created!)`
