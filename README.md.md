
# NYC Yellow Taxi Data Pipeline 🚖

This project demonstrates a modern data engineering pipeline designed using **Microsoft Fabric** to process and analyze NYC Yellow Taxi trip data. The pipeline includes data ingestion, transformation, modeling, and reporting using end-to-end Fabric services.

---

## 📊 Project Architecture

![Project Architecture](BingAPI-Page-3.drawio.png)

---

## 📁 Data Pipeline Stages

### 1. **Data Source**
- Source: NYC Taxi & Limousine Commission (TLC)
- Data Format: Parquet

### 2. **Landing Stage**
- Raw data stored in Parquet format.
- Serves as the initial storage point within Microsoft Fabric.

### 3. **Staging**
- **Tables**: `stg.nyctaxi_yellow`, `stg.taxi_zone_lookup`
- Data is copied from the landing zone using **Copy Data Activity**.
- Staging stores unrefined datasets for further transformation.

### 4. **Presentation Layer**
- **Table**: `dbo.nyctaxi_yellow`
- Data is transformed and cleaned using **Dataflow Gen2 Activity**.
- Optimized for analytics and business intelligence.

### 5. **Reporting**
- A **semantic model** is built on top of the presentation layer.
- **Power BI** is used for interactive reporting and visualizations.

---

## 🧰 Built With

- **Microsoft Fabric** (Lakehouse, Dataflows Gen2, Pipelines)
- **Parquet** File Format
- **Power BI**
- **TLC Trip Data**

---

## 🚀 How to Use

1. Clone this repository.
2. Set up your Microsoft Fabric workspace.
3. Upload Parquet files to the Lakehouse Landing zone.
4. Configure pipelines for Copy Data Activity and Dataflow Gen2.
5. Connect Power BI to the semantic model for report creation.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 👤 Author

**Gayathri Rasangika**  
Conducted using a Microsoft Fabric environment.  
[LinkedIn](#) | [Email](#)
